## Insurance Charges Prediction Project

This project explores different machine learning models to analyze and predict insurance charges using the `insurance.csv` dataset. It includes regression, classification, clustering, and pipeline implementations using Scikit-Learn.

## Project Objectives

- Predict insurance charges using regression models.
- Categorize charges for classification tasks.
- Explore patterns in the dataset using clustering.
- Build and compare pipelines to improve performance.

## Methods Used

- Linear Regression
- Logistic Regression (for binary classification)
- Polynomial Regression
- KMeans Clustering
- Scikit-Learn Pipelines
- Data preprocessing (Imputation, Encoding, Scaling)

## Performance Metrics

- Regression: R², MAE, RMSE
- Classification: Accuracy, Precision, Recall, F1-Score, Confusion Matrix
- Clustering: Inertia, Silhouette Score

## Key Insights

- Smoking status and BMI have a strong influence on insurance charges.
- Polynomial regression captured complex relationships but risked overfitting.
- Pipelines made the workflow cleaner and reproducible.
- Classification models performed well when charges were split into categories.
- Clustering revealed some group structure but not clearly separated clusters.

## Tools & Libraries

- Python
- Pandas, NumPy
- Scikit-Learn
- Matplotlib, Seaborn (optional for visualization)
- Jupyter Notebook

## How to Run

1. Clone the repo
2. Open the Jupyter Notebook
3. Run each section step-by-step to view results

## Dataset

- `insurance.csv` containing features like age, sex, bmi, children, smoker, region, and charges.

## Author

- [Ragini Sinha]

