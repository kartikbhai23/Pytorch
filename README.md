# 🧠 PyTorch Deep Learning Journey

Welcome to my **PyTorch Deep Learning** repository! This repository contains a series of interactive, clean, and highly documented Jupyter Notebooks detailing my learning path from the ground up to building and training neural networks. 

The content is based on the popular **[CampusX PyTorch YouTube Playlist](https://www.youtube.com/playlist?list=PLKnIA16_Rmvboy8bmDCjwNHgTaYH2puK7)**. Every notebook has been restructured and enhanced to match professional production standards—making it perfect for recruiters and fellow researchers to explore.

---

## 🛠️ Tech Stack & Badges

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)

---

## 📂 Repository Contents & Curriculum

The repository contains 6 structured notebooks, building concepts from basic linear algebra up to full artificial neural network classifiers:

| File Name | Topic Covered | Key Learnings |
| :--- | :--- | :--- |
| 📓 **[1.Basic.ipynb](1.Basic.ipynb)** | PyTorch Tensors Fundamentals | Mathematical operations, reshaping, indexing, inplace operations, GPU memory delegation (`cuda`), and interoperability with NumPy. |
| 📓 **[2.Pytorch-training-pipleline.ipynb](2.Pytorch-training-pipleline.ipynb)** | Manual PyTorch Pipeline | Custom weight and bias parameter initialization, manual forward pass, binary cross-entropy loss formula, and manual gradient descent step execution. |
| 📓 **[3.pytorch-nn-model.ipynb](3.pytorch-nn-model.ipynb)** | Building Models with `nn.Module` | Defining layers using PyTorch structures, subclassing `nn.Module`, parameter introspection, and visualizing networks using `torchinfo`. |
| 📓 **[4.dataset_and_dataloader.ipynb](4.dataset_and_dataloader.ipynb)** | PyTorch Data Wrappers | Subclassing `Dataset` (`__len__`, `__getitem__`), and setting up batching, shuffling, and multi-threaded loading with `DataLoader`. |
| 📓 **[5.Pytorch-training-pipleline-using-nn-module.ipynb](5.Pytorch-training-pipleline-using-nn-module.ipynb)** | Full Optimization Refactoring | Using `nn.Linear`, `nn.BCELoss`, and `torch.optim.SGD` to implement a clean training loop with automatic parameter updating. |
| 📓 **[ANN_fashion_mnist_pytorch.ipynb](ANN_fashion_mnist_pytorch.ipynb)** | Image Classification on Fashion MNIST | Training a Multi-Layer Perceptron (MLP) on 28x28 grayscale clothing images with scaling, cross-entropy loss, and categorical accuracy evaluation. |

---

## 🔧 Premium Bug Fixes & Refactoring

In addition to styling and adding descriptive markdown cells, the notebooks were debugged to fix common PyTorch pain points:

* **Broadcasting Dimension Mismatches**: Fixed a bug in `2.Pytorch-training-pipleline.ipynb` where calculating binary cross-entropy and accuracy did not squeeze output logits or reshape targets, resulting in invalid broadcasting shapes and runtime accuracy inflation.
* **Typographical Errors**: Corrected syntax errors in `3.pytorch-nn-model.ipynb` (e.g. `nn.relu()` instead of `nn.ReLU()`) and calls to non-existent class member attributes.
* **Variable References**: Resolved a bug in `4.dataset_and_dataloader.ipynb` where the labels array `y` was initialized using features data `x` (`y = torch.tensor(x)` instead of `y = torch.tensor(y)`).
* **Data Type Mismatches**: Cast training arrays to `.float()` in `5.Pytorch-training-pipleline-using-nn-module.ipynb` to prevent standard `double` NumPy features from clashing with PyTorch's default `float32` weight matrix tensors.

---

## ⚡ Setup & Installation

Follow these instructions to run the notebooks locally:

### 1. Clone the Repository
```bash
git clone https://github.com/kartikbhai23/Pytorch.git
cd Pytorch
```

### 2. Set Up Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install torch torchvision pandas numpy scikit-learn matplotlib torchinfo notebook
```

### 4. Run Jupyter Notebook
```bash
jupyter notebook
```

---

## 🎓 Acknowledgements
Special thanks to **CampusX** for their brilliant PyTorch tutorial series on YouTube.
- Playlist Link: [CampusX PyTorch Playlist](https://www.youtube.com/playlist?list=PLKnIA16_Rmvboy8bmDCjwNHgTaYH2puK7)
.