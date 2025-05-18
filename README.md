[中文README](README_zh.md) | English README

# Graph Neural Network (GNN) Tutorial

![GNN](https://img.shields.io/badge/Graph-Neural%20Network-blue)
![PyG](https://img.shields.io/badge/PyTorch-Geometric-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

This project is an introductory tutorial on Graph Neural Networks (GNNs), demonstrating basic applications through three Jupyter Notebook files covering **node classification**, **link prediction**, and **graph classification** tasks. Suitable for machine learning beginners and researchers interested in graph neural networks.

## 📌 Project Overview

Implemented using PyTorch Geometric (PyG) library, this project includes three core tasks:

| Task Type                | File                       | Description                       |
| ------------------------ | -------------------------- | --------------------------------- |
| **Node Classification**  | node_classification.ipynb  | Predict node categories in graphs |
| **Link Prediction**      | link_prediction.ipynb      | Predict edges in graphs           |
| **Graph Classification** | graph_classification.ipynb | Classify entire graph structures  |

## 🚀 Quick Start

### Environment Setup

PyG Installation:

1. Check torch and CUDA versions:

   ```python
   import torch
   print(torch.__version__)
   print(torch.version.cuda)

2. Install dependencies:

    Visit: https://pytorch-geometric.com/whl/

    For example, with pytorch=2.0.0 and CUDA 11.7:

   ![image-20250518132313200](.\images\image-20250518132313200.png)

   Install four dependencies: torch_scatter, torch_sparse, torch_cluster, torch_spline_conv:

   ![image-20250518132559838](.\images\image-20250518132559838.png)

   ```bash
   pip install torch_scatter -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch_sparse -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch_cluster -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch_spline_conv -f https://pytorch-geometric.com/whl/torch-2.0.0%2Bcu117.html
   pip install torch-geometric
   ```
   
   If network speed is slow, you can manually download the four corresponding .whl files and install them with pip. For example, in Linux with Python 3.11 environment:
   
   ```bash
   pip install torch_scatter-2.1.1+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch_sparse-0.6.18+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch_cluster-1.6.1+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch_spline_conv-1.2.2+pt20cu117-cp311-cp311-linux_x86_64.whl
   pip install torch-geometric
   ```
   
   