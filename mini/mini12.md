# =运算符

1. =和数学上的表示不同, 在C语言中表示赋值

   ```c
   #include <stdio.h>
   
   int main(void) {
       int a = 0;
       a = a + 5;
       int b = 6;
       printf("%d\n", a);
       printf("%d\n", b);
       a = b;
       b = a;
       printf("%d\n", a);
       printf("%d\n", b);
       return 0;
   }
   ```

2. =运算符的运算结果, 是被赋值的变量的数值

   ```c
   #include <stdio.h>
   
   int main(void) {
       int a = 0;
       printf("%d\n", a = a + 5);
       return 0;
   }
   ```

3. 其他运算符以及优先级可以参考第二章课件

