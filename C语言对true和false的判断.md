在C语言及其派生语言中，\0不是一个单独的转义序列，而是一个以八进制表示常数，而常数的数值为0，\0后面不能接0至7的数字，不然会视为是一个八进制的数字。

NULL和0的值都是一样的，但是为了目的和用途及容易识别的原因，NULL用于指针和对象，0用于数值。对于字符串的结尾，使用’\0’，它的值也是0，但是让人一看就知道这是字符串的结尾，不是指针，也不是普通的数值。

在不同的系统中，NULL并非总是和0等同，NULL仅仅代表空值，也就是指向一个不被使用的地址，在大多数系统中，都将0作为不被使用的地址，所以就有了类似这样的定义。但并非总是如此，也有些系统不将0地址作为NULL，而是用其他的地址，所以说，千万别将NULL和0等价起来，特别是在一些跨平台的代码中，这更是将给你带来灾难 #define NULL 0
[原文链接](https://blog.csdn.net/xingerr/article/details/71023294)


C语言中 非0即为true，null等于0 视作false



