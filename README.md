# lzma
(Unofficial) Git mirror of LZMA SDK release v19.00   https://www.7-zip.org/sdk.html   ;  used pthread for multi-thread parallel compress at:  https://github.com/sisong/lzma/tree/pthread 
# LZMA 适用于 Unix 环境多线程
编译时不添加 -D_7ZIP_ST 宏可以激活lzma的多线程编译，但是其官方只支持Windows下的多线程，本代码为支持Unix系统的多线程lzma，在C目录下增加ThreadsP.c 和ThreadsP.h 两个文件实现Unix环境的线程调用。同时编译也需要线程支持的源码文件 LzFindMt.c。若在编译时缺少定义，则缺啥补啥。
