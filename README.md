# MVAG-FL: Multi-View Attention Guided Feature Learning for Industrial Anomaly Detection

> **📌 Note:** The code is a **preliminary version** and may be somewhat messy with minor errors. We plan to refine and reformat it after the paper is accepted.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.8](https://img.shields.io/badge/python-3.8.12-blue.svg)](https://www.python.org/downloads/release/python-3812/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.1.2-ee4c2c.svg)](https://pytorch.org/)

This repository contains the official (preliminary) implementation of our paper **"MVAG-FL: Multi-View Attention Guided Feature Learning for Industrial Anomaly Detection"**. The method leverages multi-view attention mechanisms to learn discriminative features for unsupervised anomaly detection and localization.

---

## 📦 Datasets

### Real‑IAD

Real‑IAD is a new large‑scale challenging industrial anomaly detection dataset. Download it from the [official website](https://realiad4ad.github.io/Real-IAD/) and extract into `data/realiad`.

---

## 💻 Environments

Create a new conda environment and install the required packages. All experiments are trained for **50,000 iterations** on a single **NVIDIA RTX A6000** using PyTorch.

```bash
# Create and activate environment
conda create -n env python=3.8.12
conda activate env

# Install packages
pip3 install timm==0.8.15dev0 mmselfsup pandas transformers openpyxl imgaug numba numpy tensorboard fvcore accimage Ninja

pip3 install matplotlib==3.2.1 numpy==1.18.4 opencv_python_headless==4.6.0.66 pandas==1.3.5 Pillow==9.0.1 scikit_image==0.19.3 scikit_learn==0.22.2.post1

pip3 install scipy==1.4.1

pip3 install tabulate==0.9.0

pip3 install torch==1.12.0+cu113 torchvision==0.13.0+cu113

pip3 install tqdm==4.64.1

pip3 install ptflops==0.7

pip3 install timm==0.9.12

pip3 install mmdet==2.25.3

pip3 install --upgrade protobuf==3.20.1 scikit-image faiss-gpu

pip3 install adeval

pip3 install torch==2.1.2 torchvision==0.16.2 torchaudio==2.1.2 --index-url https://download.pytorch.org/whl/cu118

pip3 install fastprogress geomloss FrEIA mamba_ssm adeval fvcore==0.1.5.post20221221
