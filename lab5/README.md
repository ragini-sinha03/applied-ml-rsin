# Model Comparison for Classification Task

This project demonstrates the process of comparing two machine learning models, **Random Forest** and **AdaBoost**, to predict a target variable based on input features. The goal was to evaluate the performance of these models and determine which one generalizes better to unseen data.

## Process Overview

1. **Data Preprocessing**: 
   - Cleaned and processed the dataset.
   - Applied feature engineering to create new features.
   - Split the data into training and testing sets (80/20 split).

2. **Modeling**:
   - **Random Forest (100 Trees)**: A strong baseline model using 100 decision trees to classify the target variable.
   - **AdaBoost (100 Estimators)**: A boosting model focusing on correcting the errors of previous classifiers, with 100 estimators.

3. **Evaluation**:
   - Models were evaluated based on **Train Accuracy**, **Test Accuracy**, **Train F1 Score**, and **Test F1 Score**.
   - A confusion matrix was also generated for each model to observe the misclassifications.

## Results

### 1. Random Forest (100 Trees)
- **Train Accuracy**: 1.0000
- **Test Accuracy**: 0.8875
- **Train F1 Score**: 1.0000
- **Test F1 Score**: 0.8661
- **Confusion Matrix (Test)**: 
    ```
    [[  0  13   0]
     [  0 256   8]
     [  0  15  28]]
    ```

### 2. AdaBoost (100 Estimators)
- **Train Accuracy**: 0.8342
- **Test Accuracy**: 0.8250
- **Train F1 Score**: 0.8209
- **Test F1 Score**: 0.8158
- **Confusion Matrix (Test)**:
    ```
    [[  1  12   0]
     [  5 240  19]
     [  0  20  23]]
    ```

## Key Insights

- **Random Forest (100 Trees)** performed better overall, achieving higher test accuracy and a lower accuracy gap compared to AdaBoost.
- **AdaBoost (100 Estimators)** showed a smaller gap between train and test accuracy, indicating less overfitting but had slightly lower overall accuracy.

## Conclusion

Based on the evaluation, **Random Forest (100 Trees)** was found to be the better model in terms of generalization and accuracy. However, **AdaBoost** demonstrated minimal overfitting, which could be valuable in scenarios where you want to reduce the risk of overfitting.

## Further Improvements

- Hyperparameter tuning, such as adjusting the **learning rate** for AdaBoost, could improve its performance.
- Exploring ensemble methods, like combining **Random Forest** and **AdaBoost**, may provide even better results.

## Requirements

- Python 3.x
- `scikit-learn` library
- `pandas`
- `matplotlib` (for plotting, if necessary)

