# C++基础

## 语法与术语

### 声明\(Statement\)

一段语句的声明就是编程的动作，它必须已以号`;结束(就像英语句点结束)`

### 预处理去器指令\(Preprocessor Directive\)

`#include是预处理器指令不是程序的声明，一个预处理器指令由#号开始，它在程序编译之前被处理，需要注意的预处理器指令不是以分号结束的`

### 敏感匹配\(Case Sensitivity\)

C++是敏感匹配的，比如ROSE不等于Rose也不等于rose

## 编写C++程序的过程

第一步：编写源码文件\(`.cpp)和头文件(.h)。第二步：g++预处理器根据指令处理源码，比如(#include,#define),它们指示着编译之前要执行某些操作（例如另一个文件或替换符号）。第三步：g++编译器将源码编译为目标代码(obj,.o)，第四步：g++连接器将编译后的目标代码与其它目标代码或者静态库文件(.lib,.a)进行连接并生成可执行代码(Window的.exe,Linux由-o选项指定)。2-4步的过程称为构建。第五步：通过载入器将可执行代码和共享库文件(windows的.dll,Linux的.so)载入计算机内存。第六步：接受用户的输入，CPU执行可执行代码并输出。5-6步称为运行，如下图所示`

![CompilationProcess](/assets/CompilationProcess.png)

## C++基本程序模板

```c++
/*
 * C++基本程序模板
 */
#include <iostream>
using namespace std;
int main() {
   // Your Programming statements HERE!

   return 0;
}
```

## 基本的输入输出
#### 使用`cout <<`输出
在C++中，使用`cout`和流操作符`<<`向显示终端输出，你可以连续多次调用`<<`操作符,最后的endl相当于换行符，可以使用"\n"替代
```c++
cout << "hello" << " world, " << "again!" << endl;
cout << "hello," << endl << "one more time. " << endl << 5 << 4 << 3 << " " << 2.2 << " " << 1.1 << endl;
```

#### 使用`cin >>`输入
打印用户的输入到终端
```c++
#include <iostream>
using namespace std;
int main(){
    int firstInt;
    int secondInt;

    cout <<  "Enter first integer: ";
    cin >> firstInt;
    cout << "Enter second integer: ";
    cin >> secondInt;

    cout <<  "The first Int is " << firstInt << endl;
    cout <<  "The second Int is " << secondInt << endl;
    return 0;
}
```

## 什么是程序
程序是一系列指令（称为编程语句），它们依次执行 - 通常以顺序方式执行，如前面的示例和以下流程图所示。


![Construct_Sequential](/assets/Construct_Sequential.png)

## 什么是变量
计算机操作的数据，变量存储着程序处理的数据，之所以叫变量因为你可以改变它值，更确切的说，变量是
已命名的存储位置，它存储特定数据类型的值。换句话说，变量有名称，类型，存储着特定数据类型的值


```
// 声明变量的类型

int sum;
double radius;

// 声明多个同类型的变量

int sum, difference, product, quotient;
double area, circumference;

// 声明变量并赋值

int sum = 0;
double pi = 3.14159265;

// 声明多个同类型的变量并赋值

int firstNumber = 1, secondNumber = 2;
```

![BasicsVariable](/assets/BasicsVariable.png)

> 每个变量只可以声明一次，使用变量之前必须被声明，在程序中不能改变变量的类型


## 常量
常量是不可修改的变量，使用const关键词声明，在程序执行期间都不可变，必须在声明时初始化

```c++
const double PI = 3.1415926;  // Need to initialize
```
>常量的命名必须大写

## 基本数据类型

数据类型有四大类，整形(Integers),字符串(Characters),浮点数(Floating-point Numbers),布尔值(Boolean Numbers)

![var-1](/assets/var-1.png)
![var-2](/assets/var-2.png)

## 隐式类型转换与显式类型转换
将值从一种类型转换成另一种类型时叫做类型的转换，转换的方式有两种
1 通过编译器自动转换即隐式转换
2 利用强制类型转换运算符，将某一类型的数据转换为另外一种类型






