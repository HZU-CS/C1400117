# HW4

#### HW4问题

1. 数学知识遗漏：最大公约数、最小公倍数、进制转换
2. 逻辑复杂化
3. 对于特殊边界情况的处理
4. void main()

基础题

1. 无问题，熟悉ASCII表
2. 有个别同学进制转换出现错误，还有题目理解错误，熟悉进制转换

代码题

1. 穷举（最简单，推荐）

   ```c
   #include <stdio.h>
   
   int main(void)
   {
       int m, n, i;
       scanf("%d", &m);
       scanf("%d", &n);
       // 无需比大小
       for (i = m; i >= 1; i--)
       {
           if (m % i == 0 && n % i == 0)
           {
               break;
           }
       }
       printf("%d\n", i);
       return 0;
   }
   ```

   辗转相除法（效率最高）

   ```c
   #include <stdio.h>
   
   int main(void)
   {
       int a, b, r;
       scanf("%d %d", &a, &b);
       //如果a<b，交换a和b的值
       if (a < b)
       {
           r = a;
           a = b;
           b = r;
       }
       //辗转相除法，因为r的初始值不为0，所以while语句至少会执行一次
       //直至余数为零，跳出循环
       while (r != 0)
       {
           r = a % b;
           a = b;
           b = r;
       }
       //输出最大公约数
       printf("%d\n", a);
       return 0;
   }
   ```

   更相减损法

   ```c
   #include <stdio.h>
   
   int main(void)
   {
       int a, b;
       scanf("%d %d", &a, &b);
       while (a != b)
       {
           if (a > b)
               a -= b;
           else
               b -= a;
       }
       printf("%d", a);
       return 0;
   }
   ```

2. 穷举（最简单）

   ```c
   #include <stdio.h>
   
   int main(void)
   {
       int m, n, i;
       scanf("%d", &m);
       scanf("%d", &n);
       for (i = 1; i < m * n; i++) {
           if (i % m == 0 && i % n == 0) {
               break;
           }
       }
       printf("%d\n", i);
       return 0;
   }
   ```

   复用最大公约数（推荐）

   ```c
   #include <stdio.h>
   
   int gcd(int m, int n) {
       //可以自定义
   }
   
   int lcm(int m, int n) {
       return m * n / gcd(m, n);
   }
   
   int main(void)
   {
       int m, n;
       scanf("%d", &m);
       scanf("%d", &n);
       printf("%d\n", lcm(m, n));
       return 0;
   }
   ```

   为何？

   使用函数，模块化思想。

   好处？

   工业化，效率高->只需要提高每个部分的效率

   耦合度低->容易查错，个性化强

3. ```c
   #include <stdio.h>
   
   int main(void)
   {
       int m, n;
       scanf("%d %d", &m, &n);
       int fact = m;
       for (int i = 1; i < n; i++)
       {
           m *= fact;
       }
       printf("%d\n", m);
       return 0;
   }
   ```

4. 处理特殊条件（推荐）

   ```c
   #include <stdio.h>
   
   int main(void) {
       char a;
       scanf("%c", &a);
       if (a >= 'x') {
           a -= 23;
       } else {
           a += 3;
       }
       printf("%c\n", a);
       return 0;
   }
   ```

   处理环形问题

   ```c
   #include <stdio.h>
   
   int main(void) {
       char a;
       scanf("%c", &a);
       a = (a - 'a' + 3) % 26 + 'a';
       printf("%c\n", a);
       return 0;
   }
   ```

   a b c .... x y z | a b c .... x y z | a b c .... x y z | ....

