# SSML-Net: A Semi-Supervised Multimodal Framework for Aortic Stenosis Severity Classification

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-1.8%2B-orange.svg)]()

This repository contains the official PyTorch implementation of the paper: **"SSML-Net: A novel semi-supervised multimodal framework for Aortic Stenosis severity classification"**. 

## 📖 Introduction

Aortic stenosis (AS) is a progressive and life-threatening valvular disease that requires timely severity assessment. Current echocardiography-based assessments rely heavily on specialized expertise and are prone to inter-observer variability. 

**SSML-Net** is proposed to overcome the limitations of constrained labeled samples and insufficient exploitation of visual and label semantic information in automated deep learning methods. By effectively leveraging large-scale unlabeled echocardiograms and semantic information derived from class labels, SSML-Net achieves state-of-the-art performance for AS severity classification.

### ✨ Key Components
* **Global–Local Feature Enhancement Encoder (GLFE-Encoder):** Designed to capture both local structural cues and global contextual information.
* **Adaptive Unified Contrastive Learning (AUCL):** Performs confidence-aware sample partitioning and dynamically incorporates unconfident samples to refine the decision boundary.
* **Label Semantics-Driven Visual-Text (LSVT) Alignment:** Converts class labels into semantic text and applies a de-similarity constraint to mitigate inter-class semantic confusion. This explicitly aligns visual and textual features, enhancing fine-grained discrimination under limited annotations.

## 📊 Dataset

Experiments are conducted on the **TMED-2** (Tufts Medical Echocardiogram Dataset). 
* SSML-Net achieves higher Balanced Accuracy (BAcc) than existing deep learning methods for three-class AS severity classification.
* Please refer to the official [TMED-2 website/repository] for data access and download instructions. 

## ⚙️ Installation

1. Clone this repository:
   ```bash
   git clone [https://github.com/shanyuanyuan7/SSML-Net.git](https://github.com/shanyuanyuan7/SSML-Net.git)
   cd SSML-Net
