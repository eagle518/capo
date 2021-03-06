#  The Capo Library

C++标准库的轻量级拓展

* 支持的编译器(C++11以上): msvc(12.0ctp+), gcc(4.8.0+), clang(3.3.0+).
* 每个功能都是独立的头文件(hpp), 除了Win下的thread_local_ptr之外, 不需要编译.

##

    - build -> sln && Makefiles
    - capo  -> 所有的公开接口及实现
    - src   -> 需要编译的代码，及私有接口和实现
    - test  -> 测试用例
    - third -> 引入的第三方库

### ToDoList

    memory.alloc_pool               - 基于内存池的内存分配器
    pattern.trackable               - 遍历出所有该类型尚未销毁的对象实例
    utility.optional                - Just like boost::optional
    utility.any                     - Just like boost::any
    string.string                   - std::string的功能拓展
    stream                          - 流对象
    proofing.trace                  - 调试输出
    thread.blocking_queue           - 多线程下的blocking_queue
    thread.thread_pool              - 线程池
    delegate.signal                 - 线程安全、支持多线程异步模式的信号/槽[(?)use message loop]
    finalizer.ref_counter           - 基于引用计数的资源管理基类
    coroutine                       - 协程库
    ......