# Miniforge 


## Miniforge 搭建 tensorflow 环境

[![Miniforge Github 链接](https://img.shields.io/badge/Miniforge%20Github%20链接-green)](https://github.com/conda-forge/miniforge)  [![Conda 清华源官方教程](https://img.shields.io/badge/Conda%20清华源官方教程-green)](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/)  [![Pip 清华源官方教程](https://img.shields.io/badge/Pip%20清华源官方教程-green)](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/)

```bash
# 创建一个 python=3.12 指定位置的 tensorflow 虚拟环境
conda create --prefix=E:\ProgramData\miniforge3\envs\tensorflow python=3.12

# 查看 tensorflow 虚拟环境是否创建成功
(base) C:\Windows\System32>conda info --envs
# conda environments:
#
base                  *  E:\ProgramData\miniforge3
tensorflow               E:\ProgramData\miniforge3\envs\tensorflow

# 切换到 tensorflow 虚拟环境
(base) C:\Windows\System32>conda activate tensorflow

# 更新 pip
(tensorflow) C:\Windows\System32>python -m pip install --upgrade pip

# 将 pip 改为清华源
(tensorflow) C:\Windows\System32>pip config set global.index-url https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple
Writing to C:\Users\33695\AppData\Roaming\pip\pip.ini

# 使用 pip 安装 tensorflow cpu
(tensorflow) C:\Windows\System32>pip install tensorflow

# 使用 conda 安装 vscode jupyter 内核
(tensorflow) C:\Windows\System32>conda install ipykernel --update-deps --force-reinstall
```

