# 数组

#### 初始化

```c
#include <stdio.h>

int main(void) {
    int a[10];
    printf("%d\n", a[1]);
    return 0;
}
```

逐个赋值

```c
for (int i = 0; i < 10; i++) {
    a[i] = 0;
}
```

集成初始化

```c
int a[] = {2, 4, 6, 7, 1, 3, 5, 9, 11, 13, 23, 14, 32};
```

数组变量本⾝不能被赋值

#### 大小

```c
// sizeof(a) -> 整个数组所占据的内容的⼤⼩
// sizeof(a[0]) -> 数组中单个元素的大小
sizeof(a) / sizeof(a[0])
```

#### 二维数组