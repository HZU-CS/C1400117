# 指针

#### 函数中的数组

函数参数表中的数组实际上是指针

指针可以⽤数组的运算符[]进⾏运算

```c
#include <stdio.h>

int function(int *arr, int size) {
    for (int i = 0; i < size; i++) {
        arr[i] = i;
    }
}

int main(void) {
    int a[10] = {0};
    function(a, 10);
    for (int i = 0; i < 10; i++) {
        printf("%d", a[i]);
    }
    printf("\n");
}
```

#### 指针类型

所有指针的空间大小都是一样的

指向不同类型的指针是不能直接互相赋值的

通过void*来转换指针

#### 动态内存分配

malloc函数

```c
#include <stdlib.h>
void* malloc(size_t size);
```

分配大小可以是变量

分配完成后也不能修改大小

```c
int *a = (int*) malloc(n * sizeof(int));
a[0] = 0;
```

使用完后释放内存

```c
free(a);
```

