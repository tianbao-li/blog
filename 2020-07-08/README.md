### 1. linux 查看运行进程所在目录

    Linux在启动一个进程时，系统会在/proc下创建一个以PID命名的文件夹，在该文件夹下会有我们的进程的信息，
    其中包括一个名为exe的文件即记录了绝对路径，通过ll或ls –l命令即可查看。

    ll /proc/PID
    
    cwd 符号链接的是进程运行目录；
    
    exe 符号连接就是执行程序的绝对路径；
    
    cmdline 就是程序运行时输入的命令行命令；
    
    environ 记录了进程运行时的环境变量； 
    
    fd 目录下是进程打开或使用的文件的符号连接。

  引用/致谢：https://www.cnblogs.com/JThinking/p/9408854.html

### 2. linux系统下，安装pytorch_geometric

    我是 PyTorch 1.5.1

    $ pip install torch-scatter==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

    $ pip install torch-sparse==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

    $ pip install torch-cluster==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

    $ pip install torch-spline-conv==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.5.0.html

    $ pip install torch-geometric

    where ${CUDA} should be replaced by either cpu, cu92, cu101 or cu102 depending on your PyTorch installation.

  引用/致谢：https://github.com/rusty1s/pytorch_geometric

### 3. linux系统下，查看cuda版本

    cat  /usr/local/cuda/version.txt

### 4. linux系统下，安装pytorch

参考 引用/致谢：https://pytorch.org/get-started/locally/

### 5. linux terminal 中查找之前用过的命令

    ctrl+r  命令

### 6. conda常用命令

    conda update -n base conda        //update最新版本的conda

    conda create -n xxxx python=3.5   //创建python3.5的xxxx虚拟环境

    conda activate xxxx               //开启xxxx环境

    conda deactivate                  //关闭环境

    conda env list                    //显示所有的虚拟环境
    
### 7. PyCharm 连接服务器

    （1）安装专业版PyCharm

       引用并致谢： https://www.jianshu.com/p/4e00d0aafc52/ 

    （2）连接远程服务器

       引用并致谢： https://www.cnblogs.com/zhuminghui/p/10947930.html 

### 8. 简明Python教程 《A Byte of Python》
    中文译版在线阅读: https://bop.molun.net
    
    英文原版在线阅读: http://python.swaroopch.com/

### 9. vim常用命令
    dd          删除（剪切）光标所在整行
    yy          复制光标所在整行
    u           撤销上一步操作
    p           粘贴
    set nu      显示行号
    ?字符串     搜索该字符串
    
### 10. torch.nn.Module 简介
    torch.nn  
    https://pytorch.org/docs/stable/nn.html
    
    torch.nn.Module 源码分析  
    https://zhuanlan.zhihu.com/p/88712978
    
    pytorch教程之nn.Module类详解——使用Module类来自定义模型  
    https://blog.csdn.net/qq_27825451/article/details/90550890
    
### 11. 使用cuda训练模型时
    要保证
    既将模型放到CUDA上：         model = model.to(device)  或  model = model.cuda()
    也要将输入数据放到CUDA上：   data = data.to(device)    或  data = data.cuda()
    
### 12. windows 自带截图命令
    win + shift + s
    
### 13. matlab R2020a 安装破解教程
    http://www.zhanshaoyi.com/14416.html

### 14. 3D模型渲染为视图文件(off2view)
    
    参考链接：
    CSDN博客：https://blog.csdn.net/jorg_zhao/article/details/86309774
              https://blog.csdn.net/jorg_zhao/article/details/88345324
              blender v2.79b + blender-off-addon 2.7
    github: https://github.com/alextsui05/blender-off-addon/tree/blender/2.7
            https://github.com/WeiTang114/BlenderPhong
 
### 15. 3D模型格式转换(obj2ply)
    https://github.com/arpitmac74/Obj2ply
     
### 16. PointNet pytorch代码
    https://github.com/fxia22/pointnet.pytorch
    其中用到的 F.log_softmax 与 softmax 可以根据情况分析选择使用

### 17. 信息熵、条件熵、相对熵、交叉熵
    https://www.cnblogs.com/kyrieng/p/8694705.html

    

