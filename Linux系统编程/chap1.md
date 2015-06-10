#About The Book

* LINUX系统编程
* [美]Robert Love 著
* 祝洪凯 李妹芳 付途 译
* 关于 Robert Love 是<\<Linux Kernel Development\>>的作者，目前是google的工程师，对Linux内核和gnome做了很多贡献
* 第一章

***
* __系统调用(Syscall)__：Linux2.6之前是使用int0x80(中断)来实现系统调用的，在2.6之后的内核是使用sysentry/sysexit(32位机器)指令来实现的系统调用，这两条指令是CPU原生支持的是内核向上层库(是应用提供的接口)，API的一个特例，也是从ring3到ring0的一种方式。

***
* __API(Application Programming Interface):程序编程接口__。在我们使用一些库的时候，库提供的接口。如果两个模块
提供相同的API，则这两个模块是源码兼容，但是API如何实现，可能不一样，但是API用户都能成功编译。

***
* __ABI(Application Binary Interface):二进制接口__。它定义了应用程序内部如何交互，应用程序如何与内核交互，以及如何和库交互，保证了二进制兼容，对于同一个ABI，目标代码可以在任何系统上正常运行，而不需要重新编译。它关注的是函数调用约定，字节序，寄存器的使用，系统调用，链接，库的行为以及二进制目标的格式。ABI是操作系统和体系结构共同提供的功能。为一个体系结构定义一套ABI是比较困难的，二进制可移植比较困难的。

***

