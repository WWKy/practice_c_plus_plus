# 一个简单的String类练习
### strcpy_s不能复制0？
### [拷贝赋值函数，自赋值](https://github.com/WWKy/practice_c_plus_plus/blob/dcd5faa784d2dc62deab8d24f3cc5d66b7d600f1/string/string/String.h#L42)
 - 在写拷贝赋值函数（赋值运算符重载）时，注意考虑自赋值的情况。不然可能会出现内存泄漏、存储内容错误等情况。
### [函数参数默认值](https://github.com/WWKy/practice_c_plus_plus/blob/c66aa49dc50667b5a6e78c4ae6c48903e9193002/string/string/String.h#L16)
 - 函数参数地默认值应该在函数的声明还是定义？经测试，两者均可，但应满足以下两条：
     1. 不能重复。不能既在函数声明时指定默认值，又在函数定义时指定默认值。
     2. 若要在函数定义时指定参数默认值，函数定义必须在函数调用之前
