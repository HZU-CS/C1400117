# if判断

if语法

```c
if (条件) {
    操作
}
```

if表示如果，即满足()内的条件，那么就执行{}内的操作。

条件只有0和非0，被()包围，操作在{}中

```c
#include <stdio.h>

int main(void) {
    if (10086) {
        printf("Wow, positive\n");
    }
    if (-5) {
        printf("Wow, negative\n");
    }
    if (0) {
        printf("Wow, never print\n");
    }
}
```