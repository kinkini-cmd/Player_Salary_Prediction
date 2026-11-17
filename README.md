# Logistic Regression – Baseball Player Salary Prediction

## Project Overview

This project implements a Logistic Regression classification model using Python and Scikit-learn to predict whether a baseball player belongs to the High Salary or Low Salary category based on their performance statistics.

The original dataset contains baseball player statistics, including batting performance, career statistics, experience, and league information.

The continuous Salary variable is converted into a binary classification target using the median salary.

## Objectives

- Understand Logistic Regression for binary classification.
- Perform data preprocessing and cleaning.
- Handle missing values.
- Encode categorical variables.
- Scale numerical features.
- Train and evaluate a Logistic Regression model.
- Test the trained model using unseen data.

## Dataset

**Dataset:** Hitters.csv

The dataset includes the following features:

| Feature | Description |
|---|---|
| AtBat | Times at bat |
| Hits | Number of hits |
| HmRun | Home runs |
| Runs | Runs scored |
| RBI | Runs batted in |
| Walks | Number of walks |
| Years | Years played |
| CAtBat | Career at-bats |
| CHits | Career hits |
| CHmRun | Career home runs |
| CRuns | Career runs |
| CRBI | Career RBIs |
| CWalks | Career walks |
| League | Player's league |
| Division | Player's division |
| PutOuts | Putouts |
| Assists | Assists |
| Errors | Errors |
| NewLeague | New league |

## Target Variable

The original Salary column is converted into a binary classification variable called `HighSalary`.

- `0` – Low Salary
- `1` – High Salary

The median salary is used as the classification threshold.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Machine Learning Workflow

1. Import required libraries.
2. Load the Hitters dataset.
3. Explore dataset structure and statistical information.
4. Check and handle missing values.
5. Create the binary target variable.
6. Separate independent and dependent variables.
7. Identify numerical and categorical features.
8. Apply preprocessing.
9. Split the dataset into training and testing sets.
10. Build a Logistic Regression model.
11. Train the model.
12. Predict salary categories.
13. Evaluate model performance.
14. Test predictions using unseen data.

## Data Preprocessing

The following Scikit-learn techniques are used:

| Technique | Purpose |
|---|---|
| SimpleImputer | Handle missing values |
| StandardScaler | Standardize numerical features |
| OneHotEncoder | Encode categorical features |
| ColumnTransformer | Apply different transformations to different columns |
| Pipeline | Combine preprocessing and model training |
| train_test_split | Split training and testing data |

## Model

**Algorithm:** Logistic Regression

Logistic Regression estimates the probability of a baseball player belonging to the High Salary category.

The Sigmoid function is:

P(y = 1) = 1 / (1 + e^(-z))

Where:

z = b0 + b1x1 + b2x2 + ... + bnxn

## Model Evaluation

The model is evaluated using:

- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1-Score
- ROC-AUC Score

### Example Results

| Metric | Result |
|---|---:|
| Accuracy | 71.70% |
| ROC-AUC | 0.82 |

*Results are from one train-test split and may vary with different data splits or preprocessing.*

## Unseen Data Prediction

After training, the model is tested using new fictional baseball player statistics that were not included in the original training dataset.

The model predicts:

- Low Salary (0)
- High Salary (1)

It also calculates the probability of belonging to the High Salary category.

## Learning Outcomes

Through this project, I practiced:

- Binary classification using Logistic Regression.
- Exploratory Data Analysis (EDA).
- Handling missing values.
- Feature scaling and categorical encoding.
- Building Scikit-learn preprocessing pipelines.
- Model evaluation and performance analysis.
- Making predictions on unseen data.

## Future Improvements

- Compare Logistic Regression with Decision Tree and Random Forest.
- Perform cross-validation.
- Apply hyperparameter tuning.
- Experiment with different classification thresholds.
- Improve model performance.

## Author

**Dimalsha Kinkini**

Undergraduate Data Science Student

Sri Lanka Technological Campus (SLTC)

---

*This project was developed for educational purposes as part of my Machine Learning learning journey.*
