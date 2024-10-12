---
date: '4'
title: 'X-Ray COVID Classification - Transfer Learning'
cover: './demo.png'
external: 'https://github.com/AyoubFrihaoui/Deep-Learning-Labs/blob/main/Lab%204%20-%20Transfer%20Learning/final%20notebook.ipynb'
cta: 'https://github.com/AyoubFrihaoui/Deep-Learning-Labs/blob/main/Lab%204%20-%20Transfer%20Learning/final%20notebook.ipynb'
tech:
  - Python
  - Tensorflow
  - Keras
  - Jupyter Notebook
---

The [Chest X-ray dataset from Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) was utilized, consisting of four classes (COVID,
Lung_Opacity, Normal, Viral Pneumonia). Data preprocessing involved normalization and
a stratified hold-out strategy to split the dataset into 70% for training and 30% for
validation. Three transfer learning models were developed using the MobileNetV2
architecture with ImageNet pre-trained weights:

- Model 1: Retrained the last 3 fully connected layers.
- Model 2: Retrained the last convolutional layer and the 3 fully connected layers.
- Model 3: Retrained the last 2 convolutional layers and the 3 fully connected layers.
