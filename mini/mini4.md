# printf

1. printf是一个用来输出打印的函数, 它的用处是打印出""之内的文本

2. \n是换行符, 用于换行, 可以使得输出打印格式比较美观, 例子如下

   ```c
   #include <stdio.h>
   
   int main(void) {
       printf("Hello\n World!\n");
       return 0;
   }
   ```

3. 注意是\n而不是/n, 是从左上到右下的斜杠