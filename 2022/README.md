### 1. linux系统中删除.fuse_hidden文件

    lsof .fuse_hidden00066cdc00000025
    
    kill 对应的进程
    
### 2. 安装 Mathtype 6.9
    
    参考：https://blog.csdn.net/weixin_44198316/article/details/120692731
    
        
### 3. 安装 Typora (Windows)
    
    参考：https://www.cnblogs.com/xiaohi/p/15907083.html
    
### 4. 解决 Failed to initialize NVML: Driver/library version mismatch
    
    参考: https://blog.csdn.net/yyhaohaoxuexi/article/details/124449062
    
### 5. Python绘制频率分布直方图和条形图

    参考: https://blog.csdn.net/weixin_39505820/article/details/121993969
    
### 5. linux ubuntu系统，添加用户并赋予权限

    查看用户列表: cat /etc/passwd
    查看用户组: cat /etc/group
    创建用户且指定该用户的根路径和密码: useradd -d /home/mydir -m username
    设置密码: passwd username
    用户授权: chown -R username: username /home/ mydir
    将用户加入到组: usermod -G groupA username
    
### 6. cdo 命令 处理 .nc 文件

    拼接数据： cdo cat *.nc target_file_name.nc
    
### 6. tmux 启用鼠标

    ctrl + B : set -g mouse on
   
