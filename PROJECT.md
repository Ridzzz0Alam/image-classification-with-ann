# Fashion-MNIST Classification Project

## Dataset Overview

**Fashion-MNIST** (Zalando Research) contains 70,000 grayscale images of clothing items, each with a resolution of 28 × 28 pixels.

- **Total images:** 70,000
- **Training images:** 60,000
- **Testing images:** 10,000
- **Image size:** 28 × 28 pixels
- **Number of classes:** 10
- **Class distribution:** Perfectly balanced

### Classes

The dataset contains the following 10 clothing categories:

1. T-shirt/top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle boot

### Dataset Format

The Kaggle version is provided as a CSV file containing:

- One label column.
- 784 pixel columns per image.

The dataset is also available through:

- `keras.datasets`
- `torchvision.datasets`

### Dataset Sources

- [Fashion-MNIST on Kaggle](https://www.kaggle.com/datasets/zalando-research/fashionmnist)
- [Original Fashion-MNIST Repository (Zalando Research)](https://github.com/zalandoresearch/fashion-mnist)

---

## Task Breakdown

### Task 1: Data Exploration and Preprocessing

1. Display one sample image per class in a grid.
2. Confirm that the dataset is class-balanced.
3. Scale pixel values to the range **0–1**.
4. Flatten each image into a vector of 784 features.
5. Create a validation split from the training data.

**Expected Deliverables:**

- An image grid showing one sample from each class.
- The final array shapes for training, validation, and testing.
- One sentence explaining why pixel scaling is important for model training.

### Task 2: Build and Train a Neural Network

Build a small fully connected neural network with the following architecture:

**784 → 128 → 10**

- Input layer: 784 neurons.
- Hidden layer: 128 neurons.
- Output layer: 10 neurons with Softmax activation.

Train the model for approximately **20–40 epochs**.

Plot the following metrics for each epoch:

- Training loss vs. validation loss.
- Training accuracy vs. validation accuracy.

**Expected Deliverables:**

- Training and validation learning curves.
- 2–3 sentences describing how the gap between training and validation performance changes as the number of epochs increases.

### Task 3: Model Evaluation and Error Analysis

1. Train your chosen model configuration.
2. Evaluate the model on the test set **once**.
3. Report the test accuracy.
4. Generate a confusion matrix.
5. Calculate per-class precision and recall.
6. Display at least 10 misclassified images, including their true and predicted labels.

**Expected Deliverables:**

- Test accuracy.
- Confusion matrix.
- Per-class precision and recall.
- At least 10 misclassified images with their corresponding true and predicted labels.

---

## Submission Format

Submit a **Jupyter Notebook (`.ipynb`)** containing:

- Code implementations.
- Markdown explanations of each task.
- Visualizations and evaluation results.

**Filename Format:**

`YourName_Project09.ipynb`