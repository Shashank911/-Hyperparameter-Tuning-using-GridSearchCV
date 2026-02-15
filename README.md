# Hyperparameter Tuning using GridSearchCV
📌 Overview
This project demonstrates how to optimize a machine learning model using GridSearchCV with cross-validation.

Hyperparameter tuning was performed on a Support Vector Machine (SVM) model to improve classification performance on the Breast Cancer dataset.

🎯 Objective
The objective of this task is to:

Understand hyperparameters in machine learning

Use GridSearchCV to test multiple parameter combinations

Apply cross-validation

Compare default vs tuned model performance

Select the best-performing model configuration

📊 Dataset Information
Dataset: Breast Cancer Dataset

Problem Type: Binary Classification

Target Variable:

1 → Malignant

0 → Benign

Features: Numerical tumor measurements

This dataset is commonly used for medical classification tasks.

🛠 Tools & Libraries Used
Python

Pandas

NumPy

Scikit-learn

GridSearchCV

⚙️ Workflow Steps
Loaded the Breast Cancer dataset

Split data into training (80%) and testing (20%)

Built a Pipeline combining:

StandardScaler (feature scaling)

SVM classifier

Defined hyperparameter grid:

C (regularization parameter)

Kernel (linear, rbf)

Gamma (scale, auto)

Applied GridSearchCV with 5-fold cross-validation

Identified best hyperparameter combination

Evaluated tuned model on test dataset

Compared default SVM vs tuned SVM

🔁 Cross-Validation
5-fold cross-validation was used during tuning:

Training data was split into 5 subsets

The model was trained and validated 5 times

Average F1 Score was calculated

Best-performing hyperparameters were selected

This improves model reliability and reduces overfitting risk.

📈 Evaluation Metrics
Metric	Description
Accuracy	Overall prediction correctness
Precision	Correct positive predictions
Recall	Ability to detect actual positives
F1 Score	Balance between precision and recall

F1 Score was used as the primary optimization metric.

📊 Performance Comparison
Model	F1 Score
Default SVM	0.9861
Tuned SVM	0.9861

Both models achieved similar performance.

This indicates that the default SVM hyperparameters were already near-optimal for this dataset.

🧠 Key Insights
Hyperparameter tuning does not always drastically improve performance.

GridSearchCV confirms whether model settings are optimal.

Cross-validation ensures reliable evaluation.

Proper tuning prevents underfitting and overfitting.

📁 Repository Structure
arduino
Copy code
Hyperparameter-Tuning/
│
├── yperparameter Tuning using GridSearchCV
.ipynb
├── model_comparison_table.png
└── README.md
🚀 Concepts Demonstrated
Hyperparameters vs learned parameters

GridSearchCV

Cross-validation

Pipeline integration

Model optimization

Performance benchmarking

✅ Conclusion
Hyperparameter tuning was successfully implemented using GridSearchCV with cross-validation.

The tuned SVM model performed comparably to the default model, confirming strong baseline performance.

This task demonstrates model optimization techniques used in professional machine learning workflows.
