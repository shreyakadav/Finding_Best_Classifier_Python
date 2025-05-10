# Spam Email Classification Using Machine Learning

This project applies multiple supervised machine learning models to detect spam emails using two datasets (`spam1.csv` and `spam2.csv`). The main goal is to compare models on their ability to identify spam with high precision, especially focusing on true positive rate (TPR) at a low false positive rate (FPR) of 1%.

## 🔍 Overview

We implemented and evaluated the following classifiers:
- Naive Bayes
- Decision Tree
- Random Forest
- Logistic Regression
- Support Vector Machine (SVM)
- AdaBoost
- Neural Network (MLPClassifier)

## 🧪 Methodology

- **Data Loading & Preprocessing**: Combined two CSV datasets, standardized features using `StandardScaler`.
- **Model Training**: Trained each model using a 50/50 train-test split with stratification.
- **Evaluation Metrics**:
  - 10-fold Cross-validated AUC on training data.
  - AUC and TPR at 1% FPR on test data.
  - Visualization of sorted test labels and predicted probabilities.

## 📈 Key Results

- Calculated average AUC scores across folds for each model.
- Determined TPR when FPR is 1%, emphasizing performance in high-precision, low-false-positive applications.
- Visualized prediction probabilities vs. ground truth labels to assess model behavior.

## 📊 Visualizations

Each model outputs two scatter plots:
- Sorted test labels (spam vs. not spam)
- Predicted probabilities sorted by example index

These help in visually evaluating model calibration and separation between classes.

## 💡 Insights

This project demonstrates how different models behave under a common framework for spam detection and helps identify models best suited for highly sensitive filtering systems (e.g., email spam filters, fraud detection).

## 🛠 Technologies Used

- Python
- Scikit-learn
- NumPy
- P
