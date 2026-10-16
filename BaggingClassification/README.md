# Breast Cancer Classification using Bagging

## Project Overview

This project uses Machine Learning to classify breast cancer cases using a Bagging Classifier with a Decision Tree as the base estimator.

Bagging (Bootstrap Aggregating) is an ensemble learning technique that combines multiple models to improve prediction stability and reduce overfitting. The model is trained and evaluated using the Breast Cancer dataset.

## Technologies Used

- Python
- Pandas
- Scikit-learn

## Machine Learning Algorithms

- Decision Tree Classifier
- Bagging Classifier (Ensemble Learning)

## Dataset Information

The project uses `breast_cancer.csv`, which contains breast cancer measurements and a target column.

- **Total Records:** 569
- **Total Columns:** 31
- **Input Features:** 30
- **Target Column:** `target`

The dataset is divided into training and testing sets using an 80:20 ratio.

## Project Workflow

1. Load the dataset using Pandas.
2. Display the dataset shape and first five records.
3. Separate input features and target labels.
4. Split the dataset into training and testing sets.
5. Create a Decision Tree Classifier as the base model.
6. Build a Bagging Classifier with 10 estimators.
7. Train the model using the training dataset.
8. Predict the target labels for the test dataset.
9. Evaluate the model using accuracy and a confusion matrix.

## Model Configuration

- **Base Estimator:** Decision Tree Classifier
- **Ensemble Method:** Bagging
- **Number of Estimators:** 10
- **Test Size:** 20%
- **Random State:** 42

## Model Results

The Bagging Classifier achieved an accuracy of **95.61%** on the test dataset.

| Evaluation Metric | Result |
|---|---:|
| Dataset Records | 569 |
| Dataset Columns | 31 |
| Test Samples | 114 |
| Correct Predictions | 109 |
| Incorrect Predictions | 5 |
| Model Accuracy | 95.61% |

### Confusion Matrix

```text
[[40  3]
 [ 2 69]]
```

The confusion matrix represents:

- **True Negatives (TN):** 40
- **False Positives (FP):** 3
- **False Negatives (FN):** 2
- **True Positives (TP):** 69

The model correctly classified 109 out of 114 test samples.

## How to Run the Project

### 1. Install Python

Install Python if it is not already available on your system.

### 2. Install Dependencies

Run the following command in your terminal:

```bash
pip install -r requirements.txt
```

### 3. Prepare the Dataset

Keep `breast_cancer.csv` in the project directory so the Python script can load it.

### 4. Run the Python Script

```bash
python BaggingClassificationBreastCancer.py
```

The script displays the dataset shape, first five records, model accuracy, and confusion matrix.

## Key Learning Outcomes

- Understanding ensemble learning techniques.
- Implementing a Decision Tree Classifier.
- Applying Bagging to a classification problem.
- Splitting data into training and testing sets.
- Evaluating a classification model using accuracy and a confusion matrix.

## Future Improvements

- Compare Bagging with Random Forest and other ensemble algorithms.
- Evaluate precision, recall, and F1-score.
- Use cross-validation for more reliable performance evaluation.
- Tune model hyperparameters to improve generalization.