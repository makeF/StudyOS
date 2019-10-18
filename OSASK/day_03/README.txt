将c文件编译为机器语言
首先,使用ccl.exe从bootpack.c生成bootpack.gas
第二步,使用gas2nask.exe从bootpack.gas生成bootpack.nas.
第三步,使用nask.exe从bootpack.nas生成bootpack.obj
第四部,使用obi2bim.exe从bootpack.obj生成bootpack.bim。
最后,使用bim2hrb.exe从bootpack.bim生成bootpack.hrb

用汇编写的函数,之后还要与bootpack.obj链接,所以也需要编译成目标文件。因此将输出格式设定为WCOFF模式。另外,还要设定成32位机器语言模式。