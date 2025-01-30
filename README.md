# Generative Adversarial Networks (GANs) for Image Generation

This repository contains implementations of different types of Generative Adversarial Networks (GANs) for generating synthetic images. The models included are:

- **Basic GAN**: Generates simple 2D shapes (circles and squares) using binary vector representations.
- **Conditional GAN (cGAN)**: Generates handwritten digits based on the MNIST dataset by conditioning the generator on class labels.
- **Deep Convolutional GAN (DCGAN)**: Uses convolutional layers to generate realistic human face images using the CelebA dataset.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Models](#models)
- [Results](#results)
- [Datasets](#datasets)
- [Acknowledgements](#acknowledgements)

## Installation

To run the code, you need to have Python installed along with PyTorch and other dependencies. You will also need to download the required datasets for training and testing the models. A detailed list of dependencies and setup instructions is provided in the documentation.

## Usage

### Running the Models
Each GAN model can be trained and tested independently. The training process involves feeding real and generated data into the discriminator, updating both the generator and discriminator iteratively. Visualization tools such as Matplotlib and torchvision are used to display generated images at different training stages.

## Models

### 1. Basic GAN
A simple GAN model that generates 2D shapes. It consists of a fully connected generator and discriminator that learn to differentiate between real and generated shapes.

### 2. Conditional GAN (cGAN)
A GAN model conditioned on class labels, designed to generate specific digits from the MNIST dataset. The generator receives both random noise and label information, enabling it to generate images corresponding to the given labels. The discriminator learns to classify images as real or fake while also identifying the class labels.

### 3. Deep Convolutional GAN (DCGAN)
A more advanced GAN model using convolutional layers for image generation. It improves stability in training and enhances image quality. DCGAN is trained on the CelebA dataset to generate realistic human face images.

## Results

Generated images are visualized throughout training. The models improve in generating realistic samples over time, reducing the difference between real and synthetic data. 
- **Basic GAN**: Shows generated 2D shapes compared to real ones.
- **cGAN**: Produces digits that align with specific labels.
- **DCGAN**: Generates high-quality human face images.

## Datasets
- **MNIST Dataset**: A collection of handwritten digits used to train the cGAN model.
- **CelebA Dataset**: A large-scale dataset of celebrity faces used for training DCGAN.
- **Synthetic Shape Dataset**: Randomly generated binary vectors representing different 2D shapes used in the Basic GAN.

## Acknowledgements
- **PyTorch**: The deep learning framework used for building and training GAN models.
- **CelebA Dataset**: Used to train the DCGAN model for realistic face generation.
- **MNIST Dataset**: Used to train the cGAN model for digit generation.

This repository is open for contributions. Feel free to raise issues or suggest improvements!

