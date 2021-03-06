# 介绍

内存管理是一个非常重要的概念! 静态内存指在程序编译时, 就被设置成了一个固定长度, 在程序运行中不可改变. 但是可能存在程序的内存需求只能在运行时确定的情况. 例如, 当需要的内存取决如用户输入, 在这些情况下, 程序需要动态内存分配. C ++语言将运算符new和delete合成在一起. - 摘抄于CSDN作者: [Civil跨界工程师](https://blog.csdn.net/qq_40416052/article/details/82493916)

# 特点

1. C++通过new关键词进行动态内存分配申请.
2. C++中的动态内存分配是基于类型进行的.
3. delete关键词用于内存释放.

```cpp
TYPE *typePtr = new TYPE();
int *pNum = new int();
```

假设我们的内存条如下:

| 内存(memory) | 0    | 1    | 2    | 3    | 4    | 5    | 6    | 7    | 8    | 9    | 10   |
| ------------ | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 值(value)    |      |      | x    | x    | x    | x    |      | 2    |      |      |      |
| 名字(name)   |      |      |      |      |      |      |      | pNum |      |      |      |

假设内存条大小为10 bytes. 因为new返回的是一个pointer, 所以在内存(7)里面存的是一个内存地址. 又因为int类型的大小为4bit, 所以占用了4个byte.

# 案例

| new int;                        | 开辟一个存放整数的存储空间，返回一个指向该存储空间的地址(即指针) |
| ------------------------------- | ------------------------------------------------------------ |
| new int(100);                   | 开辟一个存放整数的空间，并指定该整数的初值为100，返回一个指向该存储空间的地址 |
| new char[10];                   | 开辟一个存放字符数组(包括10个元素)的空间，返回首元素的地址   |
| float *p = new float (3.14159); | 开辟一个存放单精度数的空间，并指定该实数的初值为//3.14159，将返回的该空间的地址赋给指针变量p |

# exception - 无法申请足够内存

C语言中, 当`malloc()`失败时会返回一个NULL指针.

C++语言中, 当`new`失败时, 会`throw exception`, 并且不会分配任何内存 - `Strong Guarantee`.

