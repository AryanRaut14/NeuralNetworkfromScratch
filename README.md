# Custom Neural Network from Scratch in PyTorch

A clean, minimalist implementation of a single-layer neural network built entirely from scratch. This project implements the forward pass, Binary Cross-Entropy (BCE) loss, backward pass, and gradient descent optimization manually using raw PyTorch tensors, without relying on high-level frameworks like `torch.nn` or `torch.optim`.


## Project Structure
* `data.csv` - The dataset containing patient clinical features and diagnostic labels.
* `Breast_Cancer_Detection.ipynb` - The Google Colab Notebook containing data preprocessing, model training, and evaluation[cite: 1].

## 🚀 Key Features
* **Custom Forward Pass:** Computes linear combinations and applies the Sigmoid activation function manually.
* **Custom Binary Cross-Entropy Loss:** Implements numerically stable BCE with manual prediction clamping to prevent log(0) errors.
* **Automatic & Manual Backward Pass Alignment:** Leverages PyTorch's Autograd engine to compute the exact analytical gradients without built-in layer abstractions.
* **Manual Optimization:** Implements vanilla Gradient Descent directly within the training loop using raw tensor gradients (`.grad`).
* **Zero Framework Overhead:** No `nn.Module`, no `nn.Linear`, and no `torch.optim` optimizers used.

