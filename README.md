# AI Task 1 – Mini ML Implementation
## Machine Failure Prediction

### Submitted by
Sagar Birajadar

### Objective
The objective of this task is to build a simple and explainable machine learning
model to predict whether an industrial machine operation will fail or not.
The focus is on correctness, clarity, and logical reasoning rather than complexity.

### Dataset Overview
The dataset contains approximately 10,000 records of industrial machine operations.
Each record includes machine type, sensor readings, and a binary failure label.

### Problem Type
Binary Classification  
Target Variable: Machine failure (0 = No Failure, 1 = Failure)

### Data Preprocessing
- Removed identifier columns such as Product ID
- Removed text-based failure description to avoid data leakage
- Encoded categorical machine type using one-hot encoding
- Performed train-test split with stratification

### Model Selection
Logistic Regression was selected because it is simple, interpretable, and suitable
for binary classification problems while meeting all task constraints.

### Model Evaluation
The model was evaluated using:
- Confusion Matrix
- Precision, Recall, F1-score
- ROC-AUC score

### Results
The model achieved a good ROC-AUC score. Tool wear time and torque were identified
as important features influencing machine failure.

### Future Improvements
- Handle class imbalance using class weights
- Try tree-based models such as Random Forest
- Apply cross-validation and feature scaling

### How to Run
1. Open the Jupyter Notebook file.
2. Ensure the dataset CSV file is in the same directory or update the file path.
3. Run all cells sequentially.
