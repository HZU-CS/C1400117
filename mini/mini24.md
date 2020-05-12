# sizeof

sizeof是⼀个运算符，给出某个类型或变量在内存中所占据的字节数，例如

```c
#include <stdio.h>

int main(void)
{
    int a = 6;
    // 类型在内存中所占据的字节数
    printf("sizeof(double)=%ld\n", sizeof(double));
    printf("sizeof(int)=%ld\n", sizeof(int));
    printf("sizeof(char)=%ld\n", sizeof(char));
    
    // 变量在内存中所占据的字节数
    printf("sizeof(a)=%ld\n", sizeof(a));
    return 0;
}
```

由于硬件不同，占据的内存空间可能会不同。

sizeof是静态运算符，它的结果在编译时刻就决定了，因此***不要在sizeof的括号⾥做运算，这些运算不会做的。***