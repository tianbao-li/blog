# 1. linux 查看运行进程所在目录

    Linux在启动一个进程时，系统会在/proc下创建一个以PID命名的文件夹，在该文件夹下会有我们的进程的信息，其中包括一个名为exe的文件即记录了绝对路径，通过ll或ls –l命令即可查看。

    ll /proc/PID

    cwd符号链接的是进程运行目录；

    exe符号连接就是执行程序的绝对路径；

    cmdline就是程序运行时输入的命令行命令；

    environ记录了进程运行时的环境变量； 

    fd目录下是进程打开或使用的文件的符号连接。


    引用/致谢：https://www.cnblogs.com/JThinking/p/9408854.html

# 2. linux系统下，安装pytorch_geometric

我是 PyTorch 1.5.1

$ pip install torch-scatter==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

$ pip install torch-sparse==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

$ pip install torch-cluster==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

$ pip install torch-spline-conv==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

$ pip install torch-geometric

where ${CUDA} should be replaced by either cpu, cu92, cu101 or cu102 depending on your PyTorch installation.

引用/致谢：https://github.com/rusty1s/pytorch_geometric

# 3. linux系统下，查看cuda版本

cat  /usr/local/cuda/version.txt

# 4. linux系统下，安装pytorch

参考 引用/致谢：https://pytorch.org/get-started/locally/

# 5. linux terminal 中查找之前用过的命令

ctrl+r  命令

# 6. conda常用命令

conda update -n base conda        //update最新版本的conda

conda create -n xxxx python=3.5   //创建python3.5的xxxx虚拟环境

conda activate xxxx               //开启xxxx环境

conda deactivate                  //关闭环境

conda env list                    //显示所有的虚拟环境

