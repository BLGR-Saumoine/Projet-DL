# Implementing Residual Networks from Scratch

![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-red) 
![Python](https://img.shields.io/badge/Python-3.10%2B-blue) 
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)

Academic project by Gendronneau Maël.

## Project Overview

This project aims to re-implement the famous Residual Network architecture (He et al., 2015) from scratch using PyTorch. The primary objective is to demonstrate the effectiveness of ResNet's residual connections compared to conventional convolutional architectures, while exploring various architectural components through systematic experimentation.

## Repository Structure

* **ResNet_Implementation.ipynb**: Main notebook containing the complete implementation, experiments, and analysis.
* **requirements.txt**: List of required dependencies (PyTorch, fastai, torchvision, etc.).
* **experiment_results/**: Directory containing saved model's performances and visualization outputs.
* **report/**: Project report documenting methodology, experiments, and conclusions.

## Key Components Implemented

### Core Architecture
- **Plain Convolutional Network**: Baseline model without residual connections
- **Residual Network**: Implementation with residual skip connections
- **Bottleneck Layers** (Optional): For deeper network configurations

### Architectural Elements
- **Residual Connections**: Identity and projection mappings
- **Batch Normalization**: With experimental comparison to models without BN
- **Modular Design**: Configurable number of layers, blocks, and normalization options

## Methodology

### Dataset
- **Imagenette**
- **Data Loading & Augmentation**: Using fastai for efficient pipeline
- **Preprocessing**: Standard ImageNet normalization and augmentation techniques

### Experiments Conducted
1. **Baseline Comparison**: Plain CNN vs. ResNet with same depth
2. **Ablation Studies**:
   - With vs. Without Batch Normalization
   - With vs. Without Residual Connections
   - Different network depths (18, 34, 50 layers)
3. **Optional Techniques** (Bag of Tricks):
   - Fully Convolutional vs. Fully Connected classification heads
   - Label Smoothing
   - Mixup Data Augmentation
   - Bottleneck Layers for deeper networks

### Implementation Details
- Pure PyTorch implementation (no high-level wrappers for core architecture)
- Custom training loops with proper validation splits
- Comprehensive logging and visualization of training dynamics
- Systematic hyperparameter tuning and comparison

## Results & Insights

The notebook presents clear experimental evidence showing:
- The impact of residual connections on gradient flow and training stability
- Batch Normalization's effect on convergence speed and generalization
- How network depth affects performance with and without residual connections
- Comparative analysis of different architectural choices

## Key References
- He et al. (2015) - Deep Residual Learning for Image Recognition
- Bag of Tricks for Image Classification (optional extensions)

## Authors
- Gendronneau Maël

*This project was completed as part of an academic curriculum in deep learning and computer vision.*
