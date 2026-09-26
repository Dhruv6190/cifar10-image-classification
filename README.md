# CIFAR-10 Image Classification using PyTorch

A convolutional neural network (CNN) built with PyTorch to classify images from the CIFAR-10 dataset into 10 categories.

## Project Overview

This project demonstrates an end-to-end image classification workflow using a CNN. It uses the CIFAR-10 dataset, applies basic image transformations, trains a neural network, and evaluates its performance on the test set.

## Dataset

The project uses **CIFAR-10**, a dataset of 60,000 colour images across 10 classes. The standard split contains 50,000 training images and 10,000 test images.

The dataset is downloaded automatically by `torchvision` when the notebook is run.

**Classes:** airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck.

## Model Architecture

The notebook defines a CNN with:

* Three convolutional layers with ReLU activations
* Max-pooling layers for spatial downsampling
* A fully connected hidden layer
* A 10-unit output layer for the class scores

The model is trained using **Cross-Entropy Loss** and the **Adam optimizer**.

## Workflow

1. Load CIFAR-10 training and test datasets.
2. Convert images to tensors and normalize the channels.
3. Create data loaders with a batch size of 32.
4. Define the CNN architecture.
5. Train the model for 10 epochs.
6. Evaluate the trained model on the test dataset.

## Repository Structure

```text
cifar10-image-classification-pytorch/
├── README.md
├── cifar10_cnn_classifier.ipynb
├── requirements.txt
└── .gitignore
```

## Requirements

* Python 3.9 or later
* PyTorch
* Torchvision
* Jupyter Notebook

Install the required packages:

```bash
pip install -r requirements.txt
```

## Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/cifar10-image-classification-pytorch.git
   cd cifar10-image-classification-pytorch
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `cifar10_cnn_classifier.ipynb` and run the cells in order.

## Results

The notebook prints the training loss for each epoch and the final test accuracy.

**Test accuracy:** Add the measured result here after running the notebook.

## Future Improvements

* Add per-class precision, recall, and F1-score.
* Plot training loss and test accuracy across epochs.
* Compare the baseline CNN with deeper architectures.
* Add sample predictions and a confusion matrix.

## Author

**Dhruv Saxena**


---

*This project is intended for learning and demonstrating a basic CNN image-classification pipeline using PyTorch.*
