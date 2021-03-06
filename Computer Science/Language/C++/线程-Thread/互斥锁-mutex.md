## 介绍

 在多任务操作系统中, 同时运行的多个线程 (thread) 可能都需要使用同一种资源.

> 比如说，同一个文件，可能一个线程会对其进行写操作，而另一个线程需要对这个文件进行读操作，可想而知，如果写线程还没有写结束，而此时读线程开始了，或者读线程还没有读结束而写线程开始了，那么最终的结果显然会是混乱的。

为了保护共享资源，在线程里也有这么一把锁 — **<u>互斥锁（mutex）</u>**，互斥锁是一种简单的加锁的方法来控制对共享资源的访问，互斥锁只有两种状态,即**上锁（lock）和解锁（unlock）**。

## `mutex`的特性

* <u>原子性 （atomic）</u>- 多个线程试图去对一个`mutex`上锁时，<u>有且只会有一个</u>线程会成功上锁。
* <u>唯一性</u> - 任何时候最多只会有一个线程锁定该`mutex`。
* <u>非繁忙等待</u> - 如果一个线程已经锁定了一个互斥量，第二个线程又试图去锁定这个互斥量，则第二个线程将被挂起（不占用任何cpu资源），直到第一个线程解除对这个互斥量的锁定为止，第二个线程则被唤醒并继续执行，同时锁定这个互斥量。

## 介绍死锁 - deadlock

当一个线程锁上了锁之后，忘记解锁了。导致其他线程只能一直处于等待状态（blocking）。这个情况下， 该锁被称为**死锁 - deadlock**。

