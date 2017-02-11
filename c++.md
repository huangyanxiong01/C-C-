# C++基础

## 语法与术语
### 声明(Statement)
一段语句的声明就是编程的动作，它必须已以号`;`结束(就像英语句点结束)

### 预处理去器指令(Preprocessor Directive)
` #include`是预处理器指令不是程序的声明，一个预处理器指令由#号开始，它在程序编译之前被处理，需要注意的预处理器指令不是以分号结束的

### 敏感匹配(Case Sensitivity)
 C++是敏感匹配的，比如ROSE不等于Rose也不等于rose

## 编写C++程序的过程  

第一步：编写源码文件(`.cpp`)和头文件(`.h`)。第二步：`g++`预处理器根据指令处理源码，比如(`#include`,`#define`),它们指示着编译之前要执行某些操作（例如另一个文件或替换符号）。第三步：g++编译器将源码编译为目标代码(`obj`,`.o`)，第四步：g++连接器将编译后的目标代码与其它目标代码或者静态库文件(`.lib`,`.a`)进行连接并生成可执行代码(Window的.exe,Linux由-o选项指定)。2-4步的过程称为构建。第五步：通过载入器将可执行代码和共享库文件(windows的`.dll`,Linux的`.so`)载入计算机内存。第六步：接受用户的输入，CPU执行可执行代码并输出。5-6步称为运行，如下图所示

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

## 最基本的输入输出
```c++

```

