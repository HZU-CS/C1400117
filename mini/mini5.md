# %d

1. printf中的%d是一种格式字符串, 表示告诉printf要往%d这个地方填一个整数

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("%d", 5);
       return 0;
   }
   ```

2. %d可以有多个, printf会按照, 后面的数挨个填入, 而且可以表示一个式子的结果

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("%d, %d, %d, %d", 5, -10, 3 + 6, 9 - 2);
       return 0;
   }
   ```

   