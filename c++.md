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








