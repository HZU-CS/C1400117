# 除法

1. 整数除法, 去掉小数部分, 例如 2 / 3 是 0, 6 / 5 是 1

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("%d", 2 / 3);
       printf("%d", 6 / 5);
       return 0;
   }
   ```

2. 要想得到小数, 一定要有一个小数参与到运算中, printf也要相应改变

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("%lf", 2 / 3.0);
       printf("%lf", 6.0 / 5);
       return 0;
   }
   ```

3. 假如有变量参与运算, 则让变量是double类型即可

   ```c
   #include <stdio.h>
   
   int main(void) {
       double a = 2;
       printf("%lf", a / 3);
       return 0;
   }
   ```

   

