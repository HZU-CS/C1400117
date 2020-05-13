# 函数调用

函数名(参数表)

```c
int function(int a, int b) {
    int res = a * a + 2 * b;
    return res;
}

int main(void) {
    function(4, 6);
    function(5, 5);
    int a = function(1, 2);
    function(function(1, 2), 3);
}
```

参数表顺序一致

函数顺序，被调用的在调用者前面

函数的参数表可以为空，但是调用一定要带上()

void类型的函数没有返回值