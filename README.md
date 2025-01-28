# Wine Type Prediction Project

## Project Overview

This project aims to predict the type of wine (red or white) based on various features such as acidity, alcohol content, sulfur dioxide levels, and others. The goal is to train and evaluate different classification models to determine which model best predicts wine type.

## Dataset

The dataset used for this project consists of two wine datasets:

- `winequality-red.csv`: Contains data for red wines.
- `winequality-white.csv`: Contains data for white wines.

Each dataset includes the following features:

- **fixed acidity**: Amount of fixed acidity in the wine.
- **volatile acidity**: Amount of volatile acidity in the wine.
- **citric acid**: Amount of citric acid in the wine.
- **residual sugar**: Amount of residual sugar in the wine.
- **chlorides**: Amount of chlorides in the wine.
- **free sulfur dioxide**: Amount of free sulfur dioxide in the wine.
- **total sulfur dioxide**: Amount of total sulfur dioxide in the wine.
- **density**: Density of the wine.
- **pH**: pH of the wine.
- **sulphates**: Amount of sulphates in the wine.
- **alcohol**: Alcohol content in the wine.
- **quality**: Quality rating of the wine (from 0 to 10).

The goal is to predict the **wine type** (`red` or `white`), which was added as a new column to the dataset.

## Steps in the Project

1. **Data Exploration and Preprocessing**
    - Load the datasets and clean the data (remove duplicates, handle missing values).
    - Combine the red and white wine datasets into a single dataset (`combined_data`).
    - Create a new column `wine_type` to distinguish between red and white wines.
    - Perform feature engineering, such as creating interaction features and encoding categorical variables.

2. **Feature Selection and Splitting the Data**
    - Define the features (all columns except `wine_type`) and target (`wine_type`).
    - Split the data into training and testing sets (80% train, 20% test).

3. **Model Selection and Evaluation**
    - Train and evaluate multiple classification models, including:
      - Logistic Regression
      - Decision Tree Classifier
      - Random Forest Classifier
    - Evaluate models using **Accuracy**.

4. **Hyperparameter Tuning**
    - Tune the hyperparameters of models to optimize performance.

5. **Feature Importance**
    - Analyze the feature importance for each model to understand the key features influencing wine type predictions.

## Results

- **Logistic Regression**: Accuracy of 0.9972
- **Decision Tree**: Accuracy of 0.9709
- **Random Forest**: Accuracy of 0.9972

The Random Forest and Logistic Regression models performed the best, achieving high accuracy.

## Future Work

- Experiment with more complex models (e.g., Support Vector Machine).
- Perform cross-validation to further evaluate model performance.
- Fine-tune hyperparameters for improved performance.

## Installation

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/betaknight/win_prediction_project.git
