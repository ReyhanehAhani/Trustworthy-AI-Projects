# Project Overview

This repository details a two-part project aimed at improving model generalization and robustness in machine learning applications. Below is an overview of each part and the techniques employed.

## Part 1: Enhancing Model Generalization

The first segment of the project focuses on training a model that achieves acceptable accuracy on both the SVHN and MNIST datasets.

### Phase 1
- **Training Data:** Used the SVHN training set.
- **Evaluation Data:** Tested on both the SVHN and MNIST test sets.
- **Methods Employed:**
  - **Pre-trained ResNet Model:** Leveraged for its robust feature-extracting capabilities.
  - **Label Smoothing:** Implemented in the loss function to help generalize better to unseen data.
  - **Data Augmentation:** To increase the diversity of the training data.

### Phase 2
- **Reverse Training Approach:**
  - **Training Data:** Switched to the MNIST training set.
  - **Testing Data:** Evaluated on both SVHN and MNIST test sets.
  - **Fine-Tuning:** Adjusted model parameters to enhance accuracy and generalization.

## Part 2: Improving Robustness Against FGSM Attacks

The second part of the project addresses the model’s defense against FGSM attacks, using the CIFAR10 dataset.

- **Adversarial Data Creation:** Developed a method to generate adversarial examples.
- **Training Conditions:**
  1. **Cross-Entropy Loss:** Standard training to establish a baseline.
  2. **Adversarial Training:** Included domain adaptation techniques with adversarial examples.
  3. **Circle Loss:** Implemented according to the method described in this [Circle Loss Paper](https://arxiv.org/abs/2002.10857).

- **Visualization:** Employed UMAP plots for better visualization and analysis of model performance under various conditions.
