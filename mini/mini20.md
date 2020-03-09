# 嵌套和级联

嵌套

```c
#include <stdio.h>

int main(void) {
    int x = 0;
    scanf("%d", &x);
    if (x > 3) {
        if (x > 6) {
            printf("x > 6\n");
        } else {
            printf("x > 3 but x <= 6\n");
        }
    } else {
        printf("x <= 3\n");
    }
    return 0;
}
```

级联

```c
#include <stdio.h>

int main(void) {
    int x = 0;
    scanf("%d", &x);
    if (x > 6) {
        printf("x > 6\n");
    } else if (x <= 3) {
        printf("x <= 3\n");
    } else {
        printf("x > 3 but x <= 6\n");
    }
    return 0;
}
```

switch代替级联，具体请参考课件。