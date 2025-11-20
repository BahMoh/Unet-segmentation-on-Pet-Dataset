# Unet-segmentation-on-Pet-Dataset

This repository contains a **PyTorch implementation of U-Net** for **binary semantic segmentation** of the Oxford-IIIT Pet dataset. The model predicts a mask for the pet in each image.

## About
U-Net is a convolutional neural network architecture for image segmentation with an encoder-decoder structure and skip connections. This project uses U-Net to segment pets from the background in images.

## Dataset
The **Oxford-IIIT Pet dataset** includes images of 37 breeds of cats and dogs along with pixel-level segmentation masks. The dataset is automatically downloaded when using `torchvision.datasets.OxfordIIITPet`.

## Dataset Structure
```bash
data/
└── oxford-iiit-pet/
    ├── images/
    │   ├── Abyssinian_1.jpg
    │   ├── Abyssinian_2.jpg
    │   ├── Birman_123.jpg
    │   ├── ... 
    │   └── yorkshire_terrier_200.jpg
    │
    └── annotations/
        ├── trimaps/
        │   ├── Abyssinian_1.png
        │   ├── Abyssinian_2.png
        │   ├── Birman_123.png
        │   ├── ...
        │   └── yorkshire_terrier_200.png
        │
        ├── xmls/
        │   ├── Abyssinian_1.xml
        │   ├── Abyssinian_2.xml
        │   ├── Birman_123.xml
        │   ├── ...
        │   └── yorkshire_terrier_200.xml
        │
        ├── trainval.txt
        ├── test.txt
        └── README
```


## Setup
Install required packages:
```bash
pip install torch torchvision numpy opencv-python pillow tqdm scikit-learn matplotlib
```
