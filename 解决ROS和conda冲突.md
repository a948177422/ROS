https://zhuanlan.zhihu.com/p/27011617

# 编辑.bashrc 顺序很重要！
# ROS
source /opt/ros/kinetic/setup.bash

# Anaconda
export PATH="/path/to/anaconda/bin:$PATH"

# 创建环境
conda create -n ros python=2 anaconda
source activate ros

# 在环境中安装依赖
pip install -U rosinstall

# 安装ROS自带cv2的依赖
conda install libgcc

