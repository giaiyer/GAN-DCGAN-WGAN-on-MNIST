# GAN, DCGAN and WGAN on MNIST Dataset

# Comparison of GAN Architectures on MNIST: MLP, DCGAN, and WGAN

This project presents a comparative study of three popular Generative Adversarial Network (GAN) architectures — **MLP-GAN**, **DCGAN**, and **WGAN** — trained on the MNIST handwritten digits dataset using PyTorch.

The goal is to explore how different GAN architectures perform in generating realistic digit images by analyzing training losses and visual outputs.

---

## Architectures Compared

### 1. MLP-GAN (Fully Connected GAN)
- Generator and Discriminator use only Linear layers.
- Suitable for basic experimentation.
- Flattens image structure.

### 2. DCGAN (Deep Convolutional GAN)
- Uses Conv2D and ConvTranspose2D layers.
- Preserves spatial structure of images.
- Produces sharper and more realistic results.

### 3. WGAN (Wasserstein GAN)
- Uses Wasserstein loss instead of binary cross-entropy.
- More stable training.
- Removes sigmoid and adds weight clipping in the discriminator.

---
## Dataset

- **MNIST**: A dataset of 28×28 grayscale images of handwritten digits (0–9).
- Automatically downloaded via `torchvision.datasets.MNIST`.
