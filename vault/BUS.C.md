---
id: ofi07erpq7jgz6mwmypxbw8
title: C-Programmierung
desc: ''
updated: 1650626027905
created: 1650538781703
---

## main
```c
#include <stdint.h>
int main(int32_t argc, char** argv)
{
    printf("Number of arguments: %d\n",argc);
    for(int i = 0; i < argc; i++)
    {
        printf("Parameter %d: %s\n",i,argv[i]);
    }
    return 0;
}
```
- Pass-by-value
- > Huch fehlgeschlagen
- `!!convert_int_to_bool`
- 