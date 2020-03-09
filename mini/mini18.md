# 条件运算符

| 运算符 | 意义     |
| ------ | -------- |
| ==     | 相等     |
| !=     | 不相等   |
| >      | 大于     |
| >=     | 大于等于 |
| <      | 小于     |
| <=     | 小于等于 |

```c
#include <stdio.h>

int main(void) {
    
    printf("%d\n", 5 == 3);
    printf("%d\n", 5 != 3);
    printf("%d\n", 5 > 3);
    printf("%d\n", 5 >= 3);
    printf("%d\n", 5 < 3);
    printf("%d\n", 5 <= 3);
    
    return 0;
}
```

也可以用于变量

```c
#include <stdio.h>

int main(void) {
    int x = 0;
    scanf("%d", &x);
    if (x < 0) {
        printf("wow, negative\n");
    }
    
    return 0;
}
```

