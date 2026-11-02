# CNN for CIFAR-10 Image Classification

## Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify images from the CIFAR-10 dataset.

The model learns visual features from images and predicts one of the 10 CIFAR-10 classes.

## Dataset

The project uses the CIFAR-10 dataset, which contains 60,000 colour images across 10 classes.

Image size: 32 × 32 pixels  
Number of classes: 10

## Model Architecture

The CNN contains three convolutional blocks followed by fully connected layers.

| Layer | Configuration |
|---|---|
| Convolution 1 | 3 input channels → 32 filters, 3 × 3 kernel, padding 1 |
| Activation | ReLU |
| Pooling | MaxPool2d(2, 2) |
| Convolution 2 | 32 → 64 filters, 3 × 3 kernel, padding 1 |
| Activation | ReLU |
| Pooling | MaxPool2d(2, 2) |
| Convolution 3 | 64 → 128 filters, 3 × 3 kernel, padding 1 |
| Activation | ReLU |
| Pooling | MaxPool2d(2, 2) |
| Flatten | 128 × 4 × 4 = 2048 features |
| Fully connected 1 | 2048 → 256 |
| Activation | ReLU |
| Output layer | 256 → 10 |

## Technologies Used

- Python
- PyTorch
- torchvision
- NumPy
- Matplotlib

## Model Performance

Test accuracy: **75.71%**

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/DeepakYadav9489/CNN-RNN.git
   ```

2. Install the required packages:

   ```bash
   pip install torch torchvision numpy matplotlib
   ```

3. Open `CNN_For_CIFAR10.ipynb` in Jupyter Notebook or Google Colab.

4. Run the notebook cells in order.

## Project File

- `CNN_For_CIFAR10.ipynb` – notebook containing the CNN implementation and evaluation.

## Future Improvements

- Apply data augmentation.
- Experiment with different CNN architectures.
- Tune hyperparameters and compare model performance.
