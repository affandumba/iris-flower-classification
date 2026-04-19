# Iris Flower Classification

## Problem Statement
Classify iris flowers into 3 species — Setosa, Versicolor and Virginica —
based on sepal and petal measurements. This is a classic multi-class
classification problem used to benchmark ML models.

## Dataset
- Iris Dataset (built into sklearn — no download needed)
- 150 samples, 4 features, 3 classes
- Perfectly balanced — 50 samples per species

## What makes this project different
Most Iris projects online use just one model. This project trains and
compares 4 different models — from simple KNN to a Neural Network —
and evaluates them all with the same metrics for a fair comparison.

## Models Used
| Model | Type |
|---|---|
| KNN | Distance based |
| SVM (RBF kernel) | Margin based |
| Random Forest | Ensemble |
| Neural Network | Deep Learning |

## Highlights
- EDA with pairplot, boxplots and correlation heatmap
- 3-way stratified split (60/20/20) — train, validation, test
- 5-Fold Cross Validation for all ML models
- Neural Network with EarlyStopping and restore_best_weights
- Training accuracy and loss curves plotted
- Confusion Matrix for all 4 models side by side
- Sample predictions with correct/wrong color coding
- Final model comparison table

## Result
| Model | Test Accuracy | CV Accuracy |
|---|---|---|
| KNN | ~97% | ~96% |
| SVM | ~97% | ~97% |
| Random Forest | ~97% | ~96% |
| Neural Network | ~97% | N/A |

## Key Finding
All 4 models achieve similar accuracy on Iris — showing that for small,
clean, linearly separable datasets, simple models like KNN perform just
as well as complex Neural Networks.

## Tools & Libraries
Python, NumPy, Pandas, Scikit-learn, TensorFlow, Keras, Matplotlib, Seaborn
