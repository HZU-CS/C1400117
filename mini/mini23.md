# break和continue

break跳出所在循环

```c
#include <stdio.h>

int main(void) {
    for (int i = 0; i < 5; i++) {
        if (i == 3) {
            // 到3为止，循环跳出
            break;
        }
        printf("%d\n", i);
    }
    return 0;
}
```

continue跳过这一轮循环，继续进行下一轮

```c
#include <stdio.h>

int main(void) {
    for (int i = 0; i < 5; i++) {
        if (i == 3) {
            // 到3不执行下面的步骤，进入下一轮
            continue;
        }
        printf("%d\n", i);
    }
    return 0;
}
```

