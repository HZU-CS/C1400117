# else

else语法

```c
else {
    操作
}
```

无法单独存在，如果不满足匹配的if的条件，那么就执行else。

```c
#include <stdio.h>

int main(void) {
    int x = 1;
    if (x > 2) {
        printf("wow, so big\n");
    } else {
        printf("wow, so small\n");
    }
}
```

