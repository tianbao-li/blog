# 1. PyCharm 连接服务器

    （1）安装专业版PyCharm

       引用并致谢： https://www.jianshu.com/p/4e00d0aafc52/ 

    （2）连接远程服务器

       引用并致谢： https://www.cnblogs.com/zhuminghui/p/10947930.html 

# 2. 简明Python教程 《A Byte of Python》
    中文译版在线阅读: https://bop.molun.net
    
    英文原版在线阅读: http://python.swaroopch.com/

# 3. vim常用命令
    dd          删除（剪切）光标所在整行
    yy          复制光标所在整行
    u           撤销上一步操作
    p           粘贴
    set nu      显示行号
    ?字符串     搜索该字符串
    
# 4. torch.nn.Module 简介
    torch.nn  
    https://pytorch.org/docs/stable/nn.html
    
    torch.nn.Module 源码分析  
    https://zhuanlan.zhihu.com/p/88712978
    
    pytorch教程之nn.Module类详解——使用Module类来自定义模型  
    https://blog.csdn.net/qq_27825451/article/details/90550890
    
# 5. 使用cuda训练模型时
    要保证
    模型是放到了CUDA上：     model = model.to(device)  或  model = model.cuda()
    输入数据放到了CUDA上：   data = data.to(device)    或  data = data.cuda()
    
