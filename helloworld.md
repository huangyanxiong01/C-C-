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
