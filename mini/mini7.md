# 整合+ - * / %和文本

1. %d可以和文本放在一起, 记住%d会依次填入, 例如

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("%d + %d=%d\n", 3, 5, 3 + 5);
       printf("%d - %d=%d\n", 3, 5, 3 - 5);
       printf("%d * %d=%d\n", 3, 5, 3 * 5);
       printf("%d / %d=%d\n", 6, 3, 6 / 3);
       return 0;
   }
   ```

2. 注意printf中要打印出%的话要使用%%

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("%d %% %d=%d", 3, 5, 3 % 5);
       return 0;
   }
   ```

   