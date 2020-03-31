# HW3

#### HW3主要问题

1. 循环输入
2. if判断
3. 语法错误（;、{}）
4. =和==
5. for和while的选择
6. 复杂逻辑

基础题：

1. 无问题

2. ```c
   while(1) {
   }
   ```

代码题：

1. ```c
   #include <stdio.h>
   
   int main(void) {
       int input = 0;
       scanf("%d", &input);
       if (input % 15 == 0) {
           printf("FizzBuzz\n");
       }
       else if (input % 3 == 0) {
           printf("Fizz\n");
       }
       else if (input % 5 == 0) {
           printf("Buzz\n");
       }
       else {
           printf("%d\n", input);
       }
       return 0;
   }
   ```

2. ```c
   #include <stdio.h>
   
   int main(void) {
       int input = 0;
       while (1) {
           scanf("%d", &input);
           if (input < 0) {
               break;
           }
           if (input % 15 == 0) {
               printf("FizzBuzz\n");
           }
           else if (input % 3 == 0) {
               printf("Fizz\n");
           }
           else if (input % 5 == 0) {
               printf("Buzz\n");
           }
           else {
               printf("%d\n", input);
           }
       }
       return 0;
   }
   ```

3. ```c
   #include <stdio.h>
   
   int main(void) {
       int input = 0, sum = 0;
       while (sum <= 100) {
           scanf("%d", &input);
           sum += input;
       }
       printf("%d", sum);
       return 0;
   }
   ```

4. ```c
   #include <stdio.h>
   
   int main(void) {
       int sum = 0;
       for (int i = 0; i <= 100; i++) {
           sum += i;
       }
       printf("%d", sum);
       return 0;
   }
   ```