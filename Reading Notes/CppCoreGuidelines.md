[![C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines/raw/master/cpp_core_guidelines_logo_text.png "C++ Core Guidelines")](https://github.com/isocpp/CppCoreGuidelines)

- [Per.19: Access memory predictably](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md#per19-access-memory-predictably)

  关于临近内存访问性能的问题，官方给出的例子有待商榷，只能说此例在大多数情况下具有代表性和合理性，因为C++二维数组是行主续存储的，那么逐行遍历应该是性能最好的。

  早些年做Matlab开发时，也有一个核心原则，其大意是：如果有嵌套循环，则应该尽量把繁忙的循环放到内层。例如当一个二维数组的行数远大于列数时，这时逐列遍历程序会有更好的性能。
  
  如果从更底层的角度去思考或许可以这样解释：相对于内存访问，机器指令频繁跳转的消耗已经占了主导（_我并不会汇编语言，这里只是打个比方_）。
  
  经过测试（MSVC 2017开启/O2优化）这个原则同样适用于C++，按照Per.19中的示例，当二维数组为200000行、2列，此时按逐列遍历的性能是逐行遍历的1.5倍左右。

  那么对于这条原则**我的建议是**：官方示例具有一定的指导意义，但仍然需要特殊情况特殊对待。更好的一个解释可以参考[MODERNES C++](http://www.modernescpp.com/index.php/c-core-guidelines-the-remaining-rules-to-performance)这篇文章中对这条原则的分析，即用std::vector和std::deque做对比。🌄




- to do