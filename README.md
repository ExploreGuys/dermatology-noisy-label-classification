# Dermatology Image Classification with Noisy Labels

## Problem Statement
This project focuses on building a robust image classification model for dermatology images where training labels are noisy and unreliable, while validation data is clean and expert-verified.

## Dataset Details
- Image size: 28×28 RGB
- Number of classes: 7
- Training labels: Noisy
- Validation labels: Clean (gold standard)

⚠️ Dataset is not included due to confidentiality.

## Approach
- Convolutional Neural Network (CNN) for image classification
- Label Smoothing used to handle noisy labels
- Clean validation data used for unbiased evaluation

## Noise Handling Strategy
Label smoothing reduces over-confidence on incorrect labels by softening target distributions, improving robustness under noisy supervision.

## Evaluation
- Accuracy on clean validation set
- Confusion Matrix
- Precision, Recall, F1-score
- Misclassification analysis
- Prediction confidence analysis

## Model Saving
The best-performing model is saved as:
best_model.pth

## Live Inference
A live inference function is provided that:
- Loads saved model weights
- Accepts new test data
- Returns accuracy when labels are available

This function is designed for real-time testing during on-campus interviews.

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook dermatology_noisy_labels.ipynb

```
Author

Yash Kumar
