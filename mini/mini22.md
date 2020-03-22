# for循环

和while循环类似，但是可以在括号内初始化计数器以及对计数器进行更改

```c
//计数器初始化;计数器判断条件;计数器变化
for (int i = 0; i < 10 ; i++) {
    循环体
}
```

例子

```c
#include <stdio.h>

int main(void) {
    int i = 0;
    while (i < 5) {
        printf("While!\n");
        i++;
    }
    for (i = 0; i < 5; i++) {
        printf("For!\n");
    }
    return 0;
}
```

死循环

```c
// for圆括号里的表达式均可以为空
for (;;) {
    
}
```

和while相比适用条件

1. 有整数计数器用for
2. 否则用while