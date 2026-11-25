# Student Depression Analysis with Logistic Regression

**Author:** Miguel Estrada

## Project Overview

This project explores a student depression dataset using Python and Machine Learning.

The objective is to perform Exploratory Data Analysis (EDA), identify patterns in the dataset, and develop a **Logistic Regression** classification model to predict the recorded depression outcome.

The project includes data preprocessing, categorical encoding, model training, evaluation, and interpretation of Logistic Regression coefficients.

> **Disclaimer:** This project is intended for educational and analytical purposes only. The model does not diagnose depression and should not be used to make clinical or consequential decisions about students.

## Objectives

- Explore the characteristics of the student depression dataset.
- Identify patterns and relationships between variables.
- Prepare the dataset for Machine Learning.
- Encode categorical variables appropriately.
- Train a Logistic Regression classification model.
- Evaluate the model using classification metrics.
- Analyze the importance and influence of model features.
- Interpret coefficients and odds ratios.

## Dataset

The project uses the following dataset:

`Student_Depression_Dataset.csv`

The dataset contains student-related information, including demographic, academic, social, and health-related variables.

Examples of variables analyzed include:

- Gender
- Age
- Family background
- Relationship status
- Marital status
- Living style
- Friend circle
- Health condition
- Home division
- CGPA
- Cost without study
- Depression

The target variable is `Depression`.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Exploratory Data Analysis (EDA)

The notebook performs several exploratory analyses to understand the dataset before training the model.

The analysis includes:

- Dataset structure and dimensions
- Data types and missing values
- Duplicate records
- Distribution of the target variable
- Numerical feature distributions
- Comparison of numerical variables across depression labels
- Analysis of categorical variables
- Correlation heatmap

The visualizations help identify patterns and relationships within the dataset.

## Data Preprocessing

Before training the model, the dataset is prepared using Scikit-learn.

The preprocessing workflow includes:

1. Separating the target variable from the predictors.
2. Encoding the target variable.
3. Identifying numerical and categorical features.
4. Handling missing numerical values using median imputation.
5. Handling missing categorical values using the most frequent category.
6. Applying One-Hot Encoding to categorical variables.
7. Standardizing numerical features using StandardScaler.
8. Splitting the dataset into training and testing sets.

The preprocessing operations are included in a Scikit-learn Pipeline to help prevent data leakage.

## Target Encoding

The target variable is encoded using an explicit mapping:

| Original value | Encoded value | Description |
|---|---:|---|
| No | 0 | The dataset records no depression |
| Yes | 1 | The dataset records depression |

The value `1` represents the positive class used by the Logistic Regression model.

## Categorical Encoding

Categorical predictor variables are transformed using