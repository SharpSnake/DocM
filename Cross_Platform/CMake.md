# CMake

# 目录
- [**Tutorial**](#tutorial)
  - [Step 1](#step-1)
  - [Step 2](#step-2)
  - [Step 3](#step-3)
  - [Step 4](#step-4)
  - [Step 5](#step-5)
- [**Visual Studio 中的 CMake 项目**](#visual-studio-中的-cmake-项目)
---

## **Tutorial**
[官方教程](https://cmake.org/cmake/help/latest/guide/tutorial/index.html)共分12步，这里仅记录一些关键知识点。

### Step 1
- 通常新建一个“构建”专用目录，并在这个路径下调用cmake，使生成的项目文件和其他中间文件不要和源码混淆在一起，方便清理和重新生成；
- 环境变量设置（`set`）必须在`configure_file`之前；
- 配置文件中的宏定义：
  - 使用`#cmakedefine`：同名变量才会生成，例如：`#cmakedefine Var1`，仅当CMakeLists.txt对`Var1`进行`set`才会生成；
  - 使用`#define`：总会生成，例如：`#define Var1 @VarX@`，会去CMakeLists.txt中找`VarX`的值；
- `target_include_directories`通常放在最后的位置；
---

### Step 2
- CMake也有“条件编译”功能，通过`option`创建条件变量（须在`configure_file`之前），它有以下几个特性：
  - 若不指定，默认为`OFF`；
  - 同样影响配置文件中的`#cmakedefine`定义；
  - 会显示在cmake-gui的参数列表中用于勾选；
  - 命令行模式下变量名前需要加`-D`，例如：`cmake ../ -DVar1=OFF`
- `list`命令的列表名可以随意命名，除了`APPEND`还有[其他](https://cmake.org/cmake/help/latest/command/list.html#command:list)很多操作；
- `target_include_directories`可以添加多个目录，多个目录用空格间隔或换行都可以；
---

### Step 3
只讲了一个知识点：
``` cmake
target_include_directories(Lib_Name INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
```
在库的CMakeLists.txt中指定：凡是使用此库的程序自动添加库目录到搜索路径；
***

### Step 4


---

### Step 5


---


## **Visual Studio 中的 CMake 项目**


