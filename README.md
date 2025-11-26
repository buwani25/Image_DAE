📷 Image Denoising Autoencoder

A lightweight Convolutional Autoencoder built to perform unsupervised image denoising on the STL-10 dataset. This project demonstrates how neural networks can learn to remove noise from images and reconstruct clean, high-quality outputs.

🚀 Overview

This project walks through:

Loading and visualizing STL-10 images (100k unlabeled + 8k test).

Adding Gaussian noise to simulate corrupted inputs.

Building a compact Conv Autoencoder for denoising.

Training with L1 Loss and evaluating using PSNR.

Visualizing Original → Noisy → Denoised results.

🧠 Model Architecture

The model consists of:

Encoder: Convolution + downsampling to learn compressed representations.

Decoder: Transposed convolutions to reconstruct clean images.

Objective: Minimize L1 loss between clean and reconstructed images.

📊 Training Metrics

Loss: L1 loss for sharp, natural reconstructions

PSNR: Quantitative measure of reconstruction quality

Visualizations: Side-by-side comparisons of model performance

🗂 Dataset

STL-10 dataset (96×96 RGB images)

100k unlabeled images for unsupervised training

8k test images for validation
Loaded via torchvision.datasets.STL10.

🛠 Technologies Used

Python

PyTorch / Torchvision

NumPy

Matplotlib

Jupyter Notebook

▶️ How to Run

Install dependencies:

pip install torch torchvision numpy matplotlib


Open the notebook:

jupyter notebook cnn-based-denoising-auto-encoder.ipynb


Run all cells to:

Load dataset

Generate noisy images

Train autoencoder

View denoising results

📌 Results

The notebook includes:

Training curves

PSNR improvements

Visual comparison:
Original → Noisy → Denoised

📄 Notebook

The full implementation is available in:
cnn-based-denoising-auto-encoder.ipynb
