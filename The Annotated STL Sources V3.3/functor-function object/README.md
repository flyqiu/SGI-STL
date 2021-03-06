## 仿函数/函数对象(functor/function object)

仿函数/函数对象：行为类似函数，可作为算法的某种策略，从实现的角度来看，仿函数是一种重载了 operator() 的 class 或 class template。

STL 仿函数应该有能力被函数配接器(function adapter)修饰，为了拥有配接能力，每一个仿函数必须定义自己的相应类型。

### 以操作数的个数划分，可分为一元和二元仿函数

* `unary_function`

`unary_function` 用来呈现一元函数的参数类型和返回值类型。

* `binary_function`

`binary_function` 用来呈现二元函数的第一参数类型、第二参数类型，以及返回值类型。

### 功能划分

> 算法类(Arithmetic)仿函数

STL 内建的 "算术类仿函数"，支持加法、减法、乘法、除法、模数和求反运算符。

> 关系运算类(Relational)仿函数

STL 内建的 "关系运算类仿函数" 支持等于、不等于、大于、大于等于、小于、小于等于六种运算。

> 逻辑运算类(Logical)仿函数

STL 内建的 "逻辑运算类仿函数" 支持了逻辑运算种的 And、Or、Not 三种运算。

> identity、select、project

将其参数原封不动地传回。为了间接性——间接性是抽象化的重要工具。


