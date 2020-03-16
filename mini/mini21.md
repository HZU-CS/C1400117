# while循环

循环，和if相同，只是执行次数有区别。while只要条件满足就会不断地操作。

```c
if (条件) {
	操作
}
while (条件) {
	操作
}
```

```c
#include <stdio.h>

int main(void) {
    int x = 10;
    if (x > 0) {
        printf("Hello World in if!\n");
    }
    while (x > 0) {
        printf("Hello World in while!\n");
        x--;
    }
    return 0;
}
```

注意死循环

```c
while (1) {
    操作
}

int x = 100;
while (x > 0) {
    x++;
}
```

