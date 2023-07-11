### 1. linux系统下，安装pytorch_geometric等 (2023.7.11)

  创建conda环境
    conda create -n conda_env_name python=3.8
    
  安装pytorch
    conda install pytorch==1.13.0 torchvision==0.14.0 torchaudio==0.13.0 pytorch-cuda=11.7 -c pytorch -c nvidia

    安装PyG
    conda install pyg -c pyg

  安装torch_scatter, torch_sparse等
    pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-1.13.0+${CUDA}.html
  where ${CUDA} should be replaced by either cpu, cu116, or cu117 depending on your PyTorch installation.

  引用/致谢：https://github.com/pyg-team/pytorch_geometric#installation
  
            https://pytorch.org/get-started/previous-versions/
        
