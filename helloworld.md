使用C++语言编写第一个程序并输出`Hello World`到终端console，这里使用ubuntu作为开发环境
## 安装开发开发环境
```bash
sudo apt-get install build-essential
```

## 构建Hellworld程序

- 编写源码

```c++
/*
 * First C++ program that says hello (hello.cpp)
 * 第一个C++语言程序，这里多行注释
 */

#include <iostream>    // 单行注释
using namespace std;

int main() {                        // 程序入口点
   cout << "hello, world" << endl;  // 打印"hello, world"
   return 0;                        // 终止main()
}                                   // main函数结束
```

- 构建可执行的代码

打开Linux的终端，切换工作目录，也可以使用IDE的工具的自动构建，但是我更加喜欢使用命令行
```bash
g++ -o hello hello.cpp
```
这里的g++是编译器，-o指定输出文件的选项，hello.cpp是源码文件

- 运行可执行代码

```bash
$ ./hello
hello, world
```
- 程序解释

```c++
#include <iostream>
using namespace std;
```
\#inlcude称为预处理器指令，预处理器指令都是以#开头，在编译前被处理,`#include <iostream>`这个指令告诉预处理器包含`iostream`头文件，支持输入输出操作。`using namespace std;`语句声明std在作为这个程序使用的默认命名空间。名称`cout`和`endl`可在这个程序使用，它门都是在std命名空间下

```c++
int main() { ... body ... }
```
定义名称main的函数，main函数是程序的入口点，该函数必须返回一个int整数的值

```c++
cout << "hello, world" << endl;
```
`cout`表示标准输出(或者是控制台输出)，`<<`符号就称为流插入操作。这里表示放入"hello, world"字符串输出到控制台。`endl`表示结束行或者新的一行，光标会被放到控制台的下一行

```c++
return 0;
```
退出main函数的执行并且返回0给操作系统，通常返回0信号表示正常的退出，非0值表示异常的退出，这一行是可选的，如果没有这一行，C++编译器会在main函数最后一行插入return 0;