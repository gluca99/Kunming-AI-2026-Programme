# Kunming AI+ Programme

### An Applied Introduction to AI with PyTorch

**Instructor:** Luca Ghafourpour, University of Cambridge

Twelve hands-on sessions taking you from tensors to training, diagnosing, and deploying your own neural networks. By the end you'll be able to build, train, and debug networks in PyTorch, use scikit-learn for classical ML and analysis, manage projects with conda, and track large-scale experiments with Weights & Biases. Two sessions will be dedicated to a brief introduction into how AI is being applied at the frontier of science.

---

## Course Aim

By the end of these twelve sessions, you will be able to:

- Build, train, and diagnose your own neural networks in PyTorch
- Use scikit-learn for classical ML and post-hoc analysis
- Manage reproducible projects with conda environments
- Track and sweep experiments with Weights & Biases
- Understand where AI is being applied at the frontier of science (PINNs, neural operators, AlphaFold, GNNs, and more)

---

## Repository Structure

Each session has its own folder containing the code and slides used on the day.

```
.
├── 01-workshop-1-foundations-tensors/
├── 02-practical-1-autograd-linear-regression/
├── 03-workshop-2-nnmodule-optim/
├── 04-practical-2-dataset-dataloader/
├── 05-workshop-3-diagnosing-training-wandb/
├── 06-practical-3-init-regularization/
├── 07-lecture-7-ai-for-science-pinns/
├── 08-lecture-8-neural-operators/
├── 09-workshop-4-cnns-unet/
├── 10-practical-4-sklearn-pca-forests/
├── 11-workshop-5-end-to-end/
├── 12-practical-5-qa-demo-next-steps/
├── environment.yml
└── README.md
```

Each session folder typically contains:

```
NN-session-name/
├── slides/        # slides used in the session (PDF / source)
├── code/          # notebooks and scripts
└── README.md      # (Optional) session-specific notes & instructions
```

---

## Schedule

| #  | Date        | Session              | Topic & what you'll learn |
|----|-------------|----------------------|----------------------------|
| 1  | Wed 13 May  | Workshop 1           | **Foundations: Conda + Tensors.** Why isolated environments matter. Creating a conda env and installing packages. PyTorch tensors as the building blocks of ML: creation, indexing, broadcasting, devices (CPU vs GPU), dtypes. |
| 2  | Mon 18 May  | Practical Workshop 1 | **Autograd from scratch. Linear regression.** Build a neural network using only tensors — no `nn.Module`, no `optim`. |
| 3  | Wed 27 May  | Workshop 2           | **`nn.Module`, activations, and `optim`.** Rebuild last session's network using PyTorch's abstractions. Activation functions (ReLU, GeLU, Tanh, …) and optimizers (SGD, momentum, Adam). |
| 4  | Mon 1 Jun   | Practical Workshop 2 | **Dataset, DataLoader, and the full training loop.** Why batching matters; writing a custom `Dataset`; shuffling, workers, GPU pipelines. |
| 5  | Mon 8 Jun   | Workshop 3           | **Diagnosing training: loss curves, bias–variance, and Wandb.** Diagnose training pathologies through loss curves. The bias–variance trade-off. Logging runs with Weights & Biases. |
| 6  | Wed 10 Jun  | Practical Workshop 3 | **Initialization and regularization.** Why bad initializations kill deep networks: LeCun, Kaiming, Xavier. Normalization, weight decay, dropout, and early stopping as forms of regularization. |
| 7  | Fri 12 Jun  | Academic Lecture 7   | **AI for Science I: The landscape and PINNs.** Traditional scientific computing vs ML for science. Physics-Informed Neural Networks (PINNs). |
| 8  | Mon 15 Jun  | Academic Lecture 8   | **AI for Science II: Neural Operators and the frontier.** Making PINNs more expressive; DeepONet, Fourier Neural Operators. A tour of the wider frontier: AlphaFold, GNNs for molecules, etc. |
| 9  | Wed 17 Jun  | Workshop 4           | **CNNs and UNet.** Convolution as a translation-equivariant operation; pooling and receptive fields. Build a small CNN and compare it to a classic neural network, then introduce the UNet. |
| 10 | Fri 19 Jun  | Practical Workshop 4 | **Classical ML with sklearn.** PCA for dimensionality reduction, random forests for feature importance, pipelines, and classical models. |
| 11 | Thu 25 Jun  | Workshop 5           | **End-to-end experiment.** A complete project tying everything together: conda env, dataloader, model, Wandb sweeps, sklearn post-hoc analysis. |
| 12 | Fri 26 Jun  | Practical Workshop 5 | **Open Q&A, AI-for-Science demo, and where to go next.** Q&A. One polished demo. Resources for continuing: Papers with Code, HuggingFace, Kaggle, NeurIPS, ICML, ICLR. |

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/gluca99/Kunming-AI-2026-Programme.git
cd kunming-ai-plus
```

### 2. Create the conda environment

```bash
conda env create -f environment.yml
conda activate kunming-ai
```

> If you don't yet have conda, install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) first. Workshop 1 covers environments in detail.

---

## Tools Used

| Tool | Purpose |
|------|---------|
| [PyTorch](https://pytorch.org/) | Building and training neural networks |
| [scikit-learn](https://scikit-learn.org/) | Classical ML and analysis |
| [conda](https://docs.conda.io/) | Reproducible environment management |
| [Weights & Biases](https://wandb.ai/) | Experiment tracking and sweeps |

---

## Where to Go Next

- **[Papers with Code](https://paperswithcode.com/)** — papers paired with implementations
- **[Hugging Face](https://huggingface.co/)** — models, datasets, and the wider ecosystem
- **[Kaggle](https://www.kaggle.com/)** — competitions and datasets to practice on
- **Conferences:** [NeurIPS](https://neurips.cc/), [ICML](https://icml.cc/), [ICLR](https://iclr.cc/)

---