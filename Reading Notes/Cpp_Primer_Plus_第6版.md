# C++ Primer Plus  第6版

- 2.1.1 如果编译器到达main函数末尾时没有遇到返回语句，则认为main函数以如下语句结尾：return 0;这条隐含的返回语句仅适用于**main**函数，而不适用于其他函。🥝

- 3.2 除了字面值，<font color=#569CD6><b>const</b></font>值也可以用来声明数组长度。🦆

- 3.4.4 列表初始化{}中，严格来讲变量类型不是必须匹配，而是不能<font color=#ff0000><b>缩窄（narrowing）</b></font>。🏰

- 4.3.5 C++11新增<font color=#ff0000><b>原始字符串</b></font>字面值（Raw string literal）：
R "delimiter( raw_characters )delimiter"，括号内的转义字符将被忽略；当希望输出括号”()”时，原始字符串必须以R"+\*(开头，以)+\*"结尾；🐆

- 4.7.5 尝试释放已经释放的内存结果是不确定的，但对空指针使用<font color=#569CD6><b>delete</b></font>是安全的。🍇

- 4.10 <font color=#4EC9B0><b>vector</b></font>的operator[]和at的区别在于后者会做越界检查并抛异常。⚖️

- 9.2.5 声明为**static**的变量（函数）具有内部链接，可以防止与其他文件中的变量（函数）发生冲突。全局变量和函数默认具有外部链接（同使用**extern**声明）。此外：
  - const全局变量也具有内部链接；
  - 所有声明于无名命名空间中的名字，即使是显式声明为 extern，均拥有内部连接。(C++11 起)；🤓

- to do
