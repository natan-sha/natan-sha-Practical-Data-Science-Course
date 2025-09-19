# Topic 5: Machine Learning Fundamentals

## 📚 Overview

Dive into the core of machine learning with supervised and unsupervised algorithms. Learn to build, evaluate, and optimize models for various prediction and classification tasks.

## 🎯 Learning Objectives

By the end of this topic, you will be able to:

- Implement supervised learning algorithms (regression and classification)
- Apply unsupervised learning techniques (clustering and dimensionality reduction)
- Evaluate model performance using appropriate metrics
- Handle overfitting and underfitting through proper validation
- Optimize hyperparameters for better model performance
- Compare and select appropriate algorithms for different problems

## 📖 Topics Covered

### 1. Supervised Learning - Regression
- Linear and polynomial regression
- Regularization techniques (Ridge, Lasso, Elastic Net)
- Tree-based methods (Decision Trees, Random Forest)
- Evaluation metrics (MSE, MAE, R²)

### 2. Supervised Learning - Classification
- Logistic regression and SVM
- Tree-based classifiers
- Naive Bayes and k-NN
- Evaluation metrics (Accuracy, Precision, Recall, F1, ROC-AUC)

### 3. Unsupervised Learning
- Clustering algorithms (K-means, Hierarchical, DBSCAN)
- Dimensionality reduction (PCA, t-SNE, UMAP)
- Association rules and market basket analysis
- Anomaly detection techniques

### 4. Model Evaluation & Validation
- Cross-validation strategies
- Bias-variance tradeoff
- Learning curves and validation curves
- Hyperparameter tuning with GridSearch and RandomSearch

## 🏗️ Project: Multi-Model Comparison Framework

Build a comprehensive framework for comparing multiple machine learning models on different datasets with automated evaluation and reporting.

### Framework Features
1. **Automated model training** pipeline
2. **Cross-validation** with multiple strategies
3. **Performance comparison** across algorithms
4. **Automated reporting** with visualizations

## 📁 Files Structure

```
topic5/
├── README.md
├── notebooks/
│   ├── 01_linear_regression.ipynb
│   ├── 02_classification_algorithms.ipynb
│   ├── 03_unsupervised_learning.ipynb
│   ├── 04_model_evaluation.ipynb
│   └── 05_model_comparison_project.ipynb
├── models/
│   ├── regression/
│   ├── classification/
│   └── unsupervised/
├── evaluation/
│   ├── metrics.py
│   ├── validation.py
│   └── comparison.py
└── assignments/
    ├── assignment_1.md
    └── assignment_2.md
```

## 🔗 Key Libraries & Tools

- **scikit-learn**: Core machine learning algorithms
- **xgboost**: Gradient boosting
- **lightgbm**: Efficient gradient boosting
- **optuna**: Hyperparameter optimization
- **mlxtend**: Extended ML utilities
- **yellowbrick**: Visual analysis

---

**Next Topic**: [Topic 6: Advanced Machine Learning](../topic6/README.md)

**Previous Topic**: [Topic 4: Feature Engineering & Selection](../topic4/README.md)
