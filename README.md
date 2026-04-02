# CIFAR-100 Efficient Deep Learning

This project explores both classification and generation on CIFAR-100 under strict constraints on model size and training time.

For classification, I built a compact CNN (~97k parameters) using MobileNet-style blocks with SE and residual connections. Trained for 10k steps, it achieves ~61% test accuracy, showing how far efficiency can be pushed with limited capacity.

For generation, I implemented a conditional GAN (<1M parameters) with residual upsampling, self-attention, and spectral normalisation. Trained for 50k steps, it achieves an FID of 28.6 and produces diverse, class-conditional samples.

The focus throughout is on the trade-off between model capacity, stability, and performance under tight constraints.