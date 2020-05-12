# char

本质上是整数

单引号表示字符的字面量：'a'，'1'

ascii表

输入输出格式：%c

```c
#include <stdio.h>

int main(void) {
    char a;
    scanf("%c", &a);
    printf("%d\n", a);
    printf("'%c'\n", a);
    return 0;
}
```

字符计算

```c
#include <stdio.h>

int main(void) {
    char c = 'A';
    c++;
    printf("%c\n", c);
    printf("%d\n", 'Z' - 'A');
    return 0;
}
```

#### 逃逸字符

| 字符 | 意义           |
| ---- | -------------- |
| \b   | 回退一格       |
| \t   | 到下一个表格位 |
| \n   | 换行           |
| \r   | 回车           |
| \\"  | 双引号         |
| \\'  | 单引号         |
| \\   | 反斜杠本身     |