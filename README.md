# Image Classification with an ANN for Fashion-MNIST

A fully connected neural network built in PyTorch with a 784 -> 128 -> 10 architecture that classifies Fashion-MNIST clothing images into 10 categories.

**Test accuracy is 88.7%**

See [`Ridwan_Project09.ipynb`](Ridwan_Project09.ipynb) for the full workflow including data exploration, preprocessing, training curves, the confusion matrix, per-class precision and recall and error analysis. The task brief is in [`PROJECT.md`](PROJECT.md).

## Setup

These commands create an isolated Python environment and install the CPU build of PyTorch together with the remaining dependencies.

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install torch --index-url https://download.pytorch.org/whl/cpu   # CPU-only build
pip install -r requirements.txt
```

## Data

The dataset is not included in this repo because of its size. Download the CSVs from [Kaggle](https://www.kaggle.com/datasets/zalando-research/fashionmnist) and place them in the folder shown below.

```
datasets/
├── fashion-mnist_train.csv
└── fashion-mnist_test.csv
```

Then open the notebook and run all cells (about 2 minutes on a CPU).
