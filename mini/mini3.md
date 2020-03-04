# 第一个程序Hello World

1. 在Visual Studio中打开.c源文件

2. 复制以下代码并运行

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("Hello World!\n");
       return 0;
   }
   ```

3. 成功看到黑色弹窗上面显示Hello World!

4. 我们前面学习大部分写程序基本在这个位置, 但是全部代码才是我们的程序

   ```c
   #include <stdio.h>
   
   int main(void) {
       我们要写程序的地方
       return 0;
   }
   ```

5. #include <stdio.h>, main, void, return 0这些我们会在后面讲解