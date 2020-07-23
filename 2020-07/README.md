# linux 查看运行进程所在目录

Linux在启动一个进程时，系统会在/proc下创建一个以PID命名的文件夹，在该文件夹下会有我们的进程的信息，其中包括一个名为exe的文件即记录了绝对路径，通过ll或ls –l命令即可查看。

ll /proc/PID

cwd符号链接的是进程运行目录；

exe符号连接就是执行程序的绝对路径；

cmdline就是程序运行时输入的命令行命令；

environ记录了进程运行时的环境变量； 

fd目录下是进程打开或使用的文件的符号连接。


引用/致谢：https://www.cnblogs.com/JThinking/p/9408854.html
