# double

输⼊输出时的格式：%lf

科学计数法：%e

```c
# include <stdio.h>

int main(void) {
    printf("%e\n", 1234.56789);
    return 0;
}
```

#### 精度

在%和f之间加上.n可以指定输出⼩数点后⼏位，这样的输出是做4舍5⼊的，例子如下

```c
# include <stdio.h>

int main(void) {
    printf("%.3f\n", -0.0049);
    printf("%.30f\n", -0.0049);
    printf("%.3f\n", -0.00049);
    return 0;
}
```

只能够通过近似和精度控制来操作，例如作差比精度小即可

#### 范围

printf输出inf表⽰超过范围的浮点数：±∞

printf输出nan表⽰不存在的浮点数

```c
# include <stdio.h>

int main(void) {
    printf("%f\n", 12.0 / 0.0);
    printf("%f\n", -12.0 / 0.0);
    printf("%f\n", 0.0 / 0.0);
    return 0;
}
```



