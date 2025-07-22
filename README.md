# Data-modification-and-generalization-in-Image-Classification

---
This repository contains the notebook `Group_24_Assignment3_Option1.ipynb`, which explores how modifying the training dataset impacts model generalization and class-wise performance in an image classification task.

---

## Project Summary

The goal of this assignment was to investigate the effect of training data manipulation on classification performance. A convolutional neural network (CNN) was trained on both **original** and **modified** versions of a dataset (likely CIFAR-10), and metrics such as **training accuracy**, **test accuracy**, and **F1 scores** were analyzed.

---

##  Key Objectives

- Compare performance on **original vs. modified datasets**
- Understand how distortions (like night-mode or blur) affect learning
- Measure model generalization by evaluating on test data
- Perform class-level analysis using **F1 scores**

---

## Files

| File Name                            | Description |
|-------------------------------------|-------------|
| `Group_24_Assignment3_Option1.ipynb` | Main notebook with training pipeline, evaluation, and insights on dataset modification effects |

---

##  Evaluation Metrics

- **Training Accuracy**: Assesses how well the model learns the modified dataset
- **Test Accuracy**: Indicates generalization to unseen data
- **F1 Score (per class)**: Highlights which classes benefit most (or least) from the training modifications

Example findings include:
- **High F1 Scores**: Airplane, Ship, Truck (≥ 80%)
- **Low F1 Scores**: Cat, Dog, Frog (≤ 60%)

These results suggest that some classes are more sensitive to distortions than others.

---

## ⚙️ Requirements

To run the notebook, install the following Python libraries:

```bash
pip install torch torchvision numpy matplotlib seaborn scikit-learn
## How to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/your-repo.git
cd your-repo
Launch Jupyter:
jupyter notebook

Key Insights
Training on modified datasets encourages the model to focus on more stable features, improving robustness under different conditions.

Some classes consistently struggle, possibly due to intra-class variability or visual similarity to other categories.

Dataset design and preprocessing choices have a direct impact on model fairness and class balance.


