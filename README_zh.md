中文README | [English README](README.md)

# Graph Neural Network (GNN) 入门教程

![GNN](https://img.shields.io/badge/Graph-Neural%20Network-blue)
![PyG](https://img.shields.io/badge/PyTorch-Geometric-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

本项目是一个 Graph Neural Network (GNN) 的入门教程，通过三个 Jupyter Notebook 文件，分别演示了 GNN 在 **节点分类**、**边预测** 和 **图分类** 任务中的基础应用。适合机器学习初学者和希望了解图神经网络的研究者。

## 📌 项目概述

本项目使用 PyTorch Geometric (PyG) 库实现，包含了以下三个核心任务：

| 任务类型     | 文件                       | 描述                 |
| ------------ | -------------------------- | -------------------- |
| **节点分类** | node_classification.ipynb  | 预测图中节点的类别   |
| **边预测**   | link_prediction.ipynb      | 预测图中边           |
| **图分类**   | graph_classification.ipynb | 对整个图结构进行分类 |

## 🚀 快速开始

### 环境配置

PyG的安装

1. 查看torch版本和cuda版本

   ```python
   import torch
   print(torch.__version__)
   print(torch.version.cuda)
   ```

2. 安装相关依赖

   https://pytorch-geometric.com/whl/

   以pytorch=2.0.0，cuda版本11.7为例：

   ![image-20250518132313200](.\images\image-20250518132313200.png)

   安装四个依赖：torch_scatter、torch_sparse、torch_cluster、torch_spline_conv：

   ![image-20250518132559838](.\images\image-20250518132559838.png)

   ```bash
   pip install torch_scatter -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch_sparse -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch_cluster -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch_spline_conv -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch-geometric
   ```

   如果网速太慢的话，也可以先手动下载四个对应的whl文件，然后用pip安装，以linux下python=3.11环境为例：

   ```bash
   pip install torch_scatter-2.1.1+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch_sparse-0.6.18+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch_cluster-1.6.1+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch_spline_conv-1.2.2+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch-geometric
   ```

