# Diffusion-Models-from-scratch

## What Are Diffusion Models?

Diffusion models are probabilistic generative models based on a forward diffusion process that incrementally adds noise to the data over several timesteps. Once the data has been corrupted into a pure noise distribution, the model is trained to reverse this process, denoising the data step by step to regenerate samples that closely match the original data distribution. These models draw inspiration from nonequilibrium thermodynamics and have been shown to produce high-quality results in tasks like image generation, density estimation, and even lossy compression.

### Diffusion Models Key Features
* Forward Process: Transforms data into a tractable Gaussian noise distribution through iterative noise addition.
* Reverse Process: Learns to denoise and reconstruct the data step by step, typically using neural networks like U-Net or simpler architectures.
* Training: Involves optimizing a variational bound to learn how to reverse the noisy data back to its original state.


## Codes

In this repository, we explore the implementation of two notable papers in diffusion models:

1. Deep Unsupervised Learning using Nonequilibrium Thermodynamics (Sohl-Dickstein et al., 2015):
    * This paper introduced the core ideas behind diffusion models. It focused on learning a generative model by progressively corrupting and then denoising data.
    * Our implementation provides a step-by-step reconstruction of the paper's diffusion process using a Multi-Layer Perceptron (MLP) architecture and Swiss Roll dataset to demonstrate key concepts.

2. Denoising Diffusion Probabilistic Models (DDPM) (Ho et al., 2020):
    * DDPM takes diffusion models to the next level with an improved U-Net architecture and an optimized loss function, yielding state-of-the-art results in image generation tasks.
    * Our implementation captures the essence of DDPM and demonstrates its power on datasets like MNIST, offering insights into the enhanced sampling and training strategies.

## References

1. Deep Unsupervised LEarning using Nonequilibrium Thermodynamics, Sohl-Dickstein et al, 2015.
2. Denoising Diffusion Probabilistic Models, Jonathan Ho et al, 2020.
3. Introduction to Diffusion Models by Maxime Vandegar<br>
URL: https://www.udemy.com/course/diffusion-models/
4. Diffusion Model from Scratch in Pytorch<br>
URL: https://towardsdatascience.com/diffusion-model-from-scratch-in-pytorch-ddpm-9d9760528946

## Additional Resources
1. The Annotated Diffusion Model<br>
URL: https://huggingface.co/blog/annotated-diffusion

