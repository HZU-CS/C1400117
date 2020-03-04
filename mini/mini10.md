# 变量

1. 储存数据的地方, 类比数学中的x, y, z等自变量

2. 程序中可以拥有多个变量

3. 变量使用声明, 声明方法是数据类型 变量名字, 数据类型暂时只需要了解int和printf

4. int表示变量是一个整数, double表示变量是一个小数, 对于小数, printf应该使用%f

   |            | printf |
   | ---------- | ------ |
   | int整数    | %d     |
   | double小数 | %lf    |

   ```c
   #include <stdio.h>
   
   int main(void) {
       int a = 10;
       printf("%d\n", a);
       double b = 1.5;
       printf("%lf\n", b);
       return 0;
   }
   ```

5. 变量类型无法中途改变

6. 变量名字必须以字母或者下划线开头, 只能包含字母, 数字和下划线, 不能使用保留字作为变量名字