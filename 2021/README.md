### 1. Matlab中 pdist 函数详解(各种距离的生成)

    D = pdist(X,distance)
    
    欧几里德距离Euclidean distance('euclidean'), 标准欧几里德距离Standardized Euclidean distance('seuclidean'), 
    夹角余弦距离Cosine distance('cosine'), Spearman distance('spearman')
    
    cite: http://blog.sciencenet.cn/blog-531885-589056.html
    
### 2. 使用指定的GPU训练模型

    torch.cuda.set_device(1)

    device = torch.device("cuda:1")

    os.environ["CUDA_VISIBLE_DEVICES"] = '1'
    os.environ["CUDA_VISIBLE_DEVICES"] = '1,2'
    
    CUDA_VISIBLE_DEVICES=1      # 只有编号为1的GPU对程序是可见的，在代码中gpu[0]指的就是这块儿GPU
    CUDA_VISIBLE_DEVICES=0,2,3  # 只有编号为0,2,3的GPU对程序是可见的，在代码中gpu[0]指的是第0块儿，gpu[1]指的是第2块儿，gpu[2]指的是第3块儿
    CUDA_VISIBLE_DEVICES=2,0,3  # 只有编号为0,2,3的GPU对程序是可见的，但是在代码中gpu[0]指的是第2块儿，gpu[1]指的是第0块儿，gpu[2]指的是第3块儿

    cite：https://blog.csdn.net/lscelory/article/details/83579062 , https://blog.csdn.net/alip39/article/details/87913543 
