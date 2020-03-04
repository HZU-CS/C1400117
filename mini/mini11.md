# scanf

1. 和printf类似, 但是是表示从键盘读入输入一个数值储存到变量中

2. Visual Studio中必须用scanf_s代替scanf, 作业中两者都可

3. 注意变量名前面要有&

   ```c
   #include <stdio.h>
   
   int main(void) {
       int a = 0;
       scanf("%d", &a);
       printf("%d\n", a);
       return 0;
   }
   ```

4. 回车表示输入完毕

5. 同样有格式字符串

   |            | scanf |
   | ---------- | ----- |
   | int整数    | %d    |
   | double小数 | %lf   |

   ```c
   #include <stdio.h>
   
   int main(void) {
       double b = 0;
       scanf("%lf", &b);
       printf("%lf\n", b);
       return 0;
   }
   ```

   