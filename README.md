# Diabetes Prediction Using Logistic Regression

## Overview

This project uses Logistic Regression to predict whether a patient is diabetic based on diagnostic measurements from the Pima Indians Diabetes Dataset.

## Dataset

The dataset is stored in `diabetes.csv`.

### Features
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

### Target
- `Outcome = 0` - Not Diabetic
- `Outcome = 1` - Diabetic

## Methodology

1. Load the diabetes dataset.
2. Define the features and target variable.
3. Split the dataset into 75% training and 25% testing data.
4. Use `random_state=16` for reproducibility.
5. Train a Logistic Regression model with `max_iter=1000`.
6. Generate predictions for the test set.
7. Create and visualize the confusion matrix.
8. Calculate accuracy and precision manually.
9. Verify the results using Scikit-learn metrics.
10. Predict diabetes for a new patient.

## Model

**Algorithm:** Logistic Regression

**Parameters:**
- `random_state=16`
- `max_iter=1000`

## Evaluation Metrics

The model is evaluated using:

- Confusion Matrix
- Accuracy
- Precision

### Accuracy

Measures the percentage of correctly classified patients.

### Precision

Measures how many patients predicted as diabetic were actually diabetic.

## Sample Prediction

The model predicts the outcome for:

```text
[2, 120, 70, 25, 80, 30.5, 0.5, 32]
```

## Requirements

```bash
pip install pandas matplotlib seaborn scikit-learn
```

## How to Run

```bash
git clone <your-repository-url>
cd diabetes-logistic-regression
python diabetes.py
```

Make sure `diabetes.csv` is present in the project directory.

## Project Structure

```text
diabetes-logistic-regression/
│
├── diabetes.csv
├── diabetes.py
└── README.md
```

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## Conclusion

Logistic Regression provides a simple classification approach for predicting diabetes from patient diagnostic measurements. The confusion matrix, accuracy, and precision help evaluate the performance of the model.

## Disclaimer

This project is intended for educational purposes only. The predictions should not be used as a substitute for professional medical diagnosis.
