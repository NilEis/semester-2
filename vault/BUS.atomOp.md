---
id: 41ubojvc0jw6nszwof6wxcm
title: Atomare Operationen
desc: ''
updated: 1653909047755
created: 1653906880487
---

- [Intel](https://cdrdv2.intel.com/v1/dl/getContent/671447)
- [AMD](https://www.amd.com/system/files/TechDocs/40332.pdf)

# Test-and-set: TSL instruction
## Implementierung des Betretens und Verlassen eines kritischen Bereichs
### C
```c
bool test_and_set(bool* target)
{
    bool res = *target;
    *target = true;
    return res;
}
```
### Assembler
```asm
enter_region:
    tsl register, lock
    cmp register, #0
    jnz enter_region

    ret

leave_region:
    mov lock, #0
    ret
```
# Swap
### C
```c
key = true;
while(key==true)
{
    swap(&lock, &key);
}
/* Kritischer Bereich */
lock = false;
```
### Assembler
```asm
enter_region:
    mov register, #1
    xchg register, lock
    cmp register, #0
    jne enter_region

    ret

leave_region:
    mov lock, #0
    ret
```
# Wait und signal
### c
```c
s = 1;
while(s)
{
    while(s==0)
    {
        __asm("nop");
    }
    s=s-1;
}

void signal()
{
    s = s + 1;
}
```
### Assembler
```asm
mutex_lock:
    tsl register, mutex
    cmp register, #0
    jze ok
    call thread_yield
    jmp mutex_lock
ok:
    ret

leave_region:
    mov mutex, #0
```
