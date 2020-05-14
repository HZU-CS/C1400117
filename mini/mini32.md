# 指针

指针，就是保存地址的变量

输入输出格式：%p

```c
int i;
int *p = &i;
```

指针变量的值是内存的地址

#### *和&

互为反操作

&取地址

针对变量

传递给函数或者指针

*取值

针对指针

修改地址上的值

#### 在函数中的应用

```c
#include <stdio.h>

void function1(int a) {
    a = 100;
}

void function2(int *a) {
    *a = 100;
}

int main(void) {
    int a = 0;
    function1(a);
    printf("After function1, a = %d\n", a);
    function2(&a);
    printf("After function2, a = %d\n", a);
    *(&a) = 10;
    printf("%d\n", a);
    return 0;
}
```

#### 常见错误

直接给指针赋值常量

```c
int *p = 5;
```

定义了指针变量，还没有指向任何变量，就开始使⽤指针