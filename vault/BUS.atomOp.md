---
id: 41ubojvc0jw6nszwof6wxcm
title: Atomare Operationen
desc: ''
updated: 1653907095014
created: 1653906880487
---

# Test-and-set: TSL instruction
## Implementierung des Betretens und Verlassen eines kritischen Bereichs
```as
enter_region:
    tsl register, lock
    cmp register, #0
    jnz enter_region

    ret

leave_region:
    mov lock, #0
    ret
```
