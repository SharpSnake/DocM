## 2024.09.10
- boost_locale可选择icu进行编码转换
- wchar_t不是定宽的，windows下是16位，linux下是32位
- GB18030、GBK等编码指的是ANSI

## 2024.09.09
- 构造函数默认具备隐式转换，除非加`explicit`标记

## 2024.09.01
- `std::atexit`是压栈，可注册lambda
- 代码文件推荐UTF-8编码（VS对应 文件->高级保存选项，linux对应编辑器的Encoding菜单），否则不能正常打印中文

## 2024.08.26
- 坏掉的istream要结合clear和ignore才能复原

## 2024.08.24
- 静态变量在main之前初始化
- C++逗号运算符

## 2024.08.22
- CI & vcpkg
- source指令运行脚本，在当前环境下立即生效，有别于直接运行脚本
