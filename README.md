# Unet-segmentation-on-Pet-Dataset

This repository contains a **PyTorch implementation of U-Net** for **binary semantic segmentation** of the Oxford-IIIT Pet dataset. The model predicts a mask for the pet in each image.

## About
U-Net is a convolutional neural network architecture for image segmentation with an encoder-decoder structure and skip connections. This project uses U-Net to segment pets from the background in images.

## Dataset
The **Oxford-IIIT Pet dataset** includes images of 37 breeds of cats and dogs along with pixel-level segmentation masks. The dataset is automatically downloaded when using `torchvision.datasets.OxfordIIITPet`.

## Dataset Structure
```bash
data/
├── images/
│ ├── Abyssinian_1.jpg
│ └── ...
└── annotations/
├── Abyssinian_1.png
└── ...
```
