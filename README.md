# Denoising Diffusion Probabilistic Models (DDPM)

## Overview
Denoising Diffusion Probabilistic Models (DDPM) are a class of generative models that learn to generate data by reversing a diffusion process. They have gained popularity for their ability to produce high-quality samples in various domains, including images, audio, and text.

## Key Concepts
1. **Diffusion Process**: This is a process where data is gradually corrupted by noise over a series of steps. The model learns to reverse this process, effectively denoising the data.
2. **Training**: The model is trained on a dataset by simulating the diffusion process and learning to predict the original data from the noisy version at each step.
3. **Sampling**: Once trained, the model can generate new samples by starting from random noise and applying the learned reverse diffusion process.

## Processes
### 1. Training Process

- **Noise Addition**: Gradually add noise to the data over a fixed number of steps, creating a series of noisy images.
- **Model Training**: Train the model to predict the original data from the noisy versions using a loss function that measures the difference between the predicted and actual data.

### 2. Sampling Process
- **Initialization**: Start with a sample of random noise.
- **Reverse Diffusion**: Iteratively apply the learned model to denoise the sample, gradually transforming it into a coherent output.
- **Output Generation**: The final output is a generated sample that resembles the training data.

## Installation
To install the required dependencies, run:
```bash
pip install -r requirements.txt
```

## Usage
To run the DDPM model, execute:
```bash
python ddpm.py
```

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- [Original Paper](https://arxiv.org/abs/2006.11239) - Denoising Diffusion Probabilistic Models


---
