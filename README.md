# 15-445/645 C++ Bootcamp
这个训练营旨在为现代 C++ 编程提供一个基础入门。
C++ 语言特性非常庞大，不可能在一次训练营中全部覆盖；而且坦白说，最好的学习方式还是实践。
课程团队相信，15-445 会让你成为更自信的 C++ 程序员！
不过，我们确实会讲解一些完成编程作业时必须掌握的 C++ 主题。
本教程不会覆盖基础 C/C++ 语法，主要聚焦于 C++ 编程特性，尤其是 C 中不存在的概念。

欢迎随时为这个 C++ bootcamp 提反馈！你可以提交 issue 或 PR。

## 组织形式
训练营由位于 `src/` 下的一组 C++ 源码文件组成，建议深入阅读。
每个文件都可以编译成一个同名可执行程序。
请使用 CMake 构建这些可执行文件。
下面这组命令会构建全部可执行程序。运行完成后，可执行文件会在 `build` 目录中。

```console
$ mkdir build
$ cd build
$ cmake ..
$ make -j8
```

例如，`src/references.cpp` 会被编译为位于 `./build` 下的 `references` 可执行文件。
`src/` 目录中的其他文件同理。

## 文件说明
`src/` 目录中共有十五个（以及一个示例）主题文件，分别讲解不同概念。
建议按下列顺序阅读，因为后面的内容会建立在前面的基础上。
当然，如果你已经了解部分现代 C++ 概念，想快速复习，也可以直接从不熟悉的主题开始。

### 引用与移动语义
- `references.cpp`：讲解 C++ 引用。
- `move_semantics.cpp`：讲解 C++ 移动语义。
- `move_constructors.cpp`：讲解 C++ 类的移动构造函数与移动赋值运算符。

### C++ 模板
- `templated_functions.cpp`：讲解 C++ 函数模板。
- `templated_classes.cpp`：讲解 C++ 类模板。

### 杂项
- `wrapper_class.cpp`：讲解 C++ 包装类（wrapper class）。
- `iterator.cpp`：讲解如何实现基础的 C++ 风格迭代器。
- `namespaces.cpp`：讲解 C++ 命名空间。

### C++ 标准库（STL）容器
- `vectors.cpp`：讲解 `std::vector`。
- `set.cpp`：讲解 `std::set`。
- `unordered_map.cpp`：讲解 `std::unordered_map`。
- `auto.cpp`：讲解 C++ 关键字 `auto` 的使用，包括如何用 `auto` 遍历 STL 容器。

### C++ 标准库（STL）内存管理
- `unique_ptr.cpp`：讲解 `std::unique_ptr`。
- `shared_ptr.cpp`：讲解 `std::shared_ptr`。

### C++ 标准库（STL）同步原语
- `mutex.cpp`：讲解 `std::mutex`。
- `scoped_lock.cpp`：讲解 `std::scoped_lock`。
- `condition_variable.cpp`：讲解 `std::condition_variable`。
- `rwlock.cpp`：讲解如何组合多个 C++ STL 同步原语库（`std::shared_mutex`、`std::shared_lock`、`std::unique_lock`）实现读写锁。

### 15-445/645 Bootcamp 演示代码
- `spring2024/s24_my_ptr.cpp`：讲解 2024 年春季 bootcamp 使用的示例代码。

## 其他资源
在你逐步熟悉 C++ 的过程中，下面这些资源会很有帮助：

- [https://en.cppreference.com/w/](https://en.cppreference.com/w/)：非官方但非常准确的 C++/C 标准摘要与示例。
- [https://cplusplus.com/](https://cplusplus.com/)：包含 C++ 语言[教程](https://cplusplus.com/doc/tutorial/)和 C++ 库[参考手册](https://cplusplus.com/reference/)。
- [Modern C++ Tutorial](https://github.com/changkun/modern-cpp-tutorial)：该 GitHub 仓库包含有用的资料与练习。

## 附录：训练营主题对应的 C++ 官方文档
这些文档可能会非常有用！内容很全面（比本训练营全面得多），但可读性可能不如教程。
总体来说，尤其在做项目时，仍然建议你尝试阅读并理解这些文档。
训练营虽尽量覆盖常见场景，但仍然只是现代 C++ 的基础入门。

- [References](https://en.cppreference.com/w/cpp/language/reference)
- [std::move](https://en.cppreference.com/w/cpp/utility/move)
- [Move Constructors](https://en.cppreference.com/w/cpp/language/move_constructor) and [Move Assignment Operators](https://en.cppreference.com/w/cpp/language/move_assignment)
- [Templated Functions](https://en.cppreference.com/w/cpp/language/function_template)
- [Templated Classes](https://en.cppreference.com/w/cpp/language/class_template)
- [Iterators](https://en.cppreference.com/w/cpp/iterator)
- [Namespaces](https://en.cppreference.com/w/cpp/language/namespace)
- [std::vector](https://en.cppreference.com/w/cpp/container/vector)
- [std::set](https://en.cppreference.com/w/cpp/container/set)
- [std::unordered_map](https://en.cppreference.com/w/cpp/container/unordered_map)
- [auto](https://en.cppreference.com/w/cpp/language/auto)
- [std::unique_ptr](https://en.cppreference.com/w/cpp/memory/unique_ptr)
- [std::shared_ptr](https://en.cppreference.com/w/cpp/memory/shared_ptr)
- [std::mutex](https://en.cppreference.com/w/cpp/thread/mutex)
- [std::scoped_lock](https://en.cppreference.com/w/cpp/thread/scoped_lock)
- [std::condition_variable](https://en.cppreference.com/w/cpp/thread/condition_variable)
- [std::shared_mutex](https://en.cppreference.com/w/cpp/thread/shared_mutex)
- [std::shared_lock](https://en.cppreference.com/w/cpp/thread/shared_lock)
- [std::unique_lock](https://en.cppreference.com/w/cpp/thread/unique_lock)
