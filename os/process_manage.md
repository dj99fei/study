#进程通信

###SYSTEM V

信号量、消息队列、共享内存是unix/linux常用的进程通信方式。
三种方式在系统中是作为一个整体实现的。其中共享内存方式的效率最高。

#死锁

死锁是并发进程约束条件处理不当产生的最严重的后果。根本原因是因为系统资源的有限性。

死锁产生的四个条件：

1.并发进程互斥，每个进程必须独占某个系统资源
2.不主动释放，除非达到目的
3.分配方式是部分分配而不是一次性分配
4.各个占有资源的进程形成环路

#线程

线程是进程内的基本调度单位。针对进程切换开销巨大于是有了线程。线程不同于进程，它只有栈段和上下文，而没有单独的数据段和程序段，而是和其他线程共享。

按照系统管理策略线程可以分为用户级线程和系统级线程。

