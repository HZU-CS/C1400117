# int

输⼊输出时的格式：%d

范围：一般来说，-2<sup>31</sup> ~ 2<sup>31</sup>-1

如果操作使得数据超过了他们的范围，那么就会溢出出错，如下面的代码

```c
#include <stdio.h>

int main(void)
{
    int a = 99999999999999999999;
    printf("%d\n", a);
    return 0;
}
```

#### unsigned

在整形类型前加上unsigned使得它们成为⽆符号的整数，注意unsigned并没有改变数据内部的⼆进制表达没变，变的是如何看待它们。

%o⽤于8进制，%x⽤于16进制。

```c
#include <stdio.h>

int main(void)
{
    unsigned int b = -1;
    printf("%u\n", b);
    int c = 10;
    printf("%o, %x\n", c, c);
    return 0;
}
```

