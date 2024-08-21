# NASA Nearest Earth Objects Prediction

## Project Description
This project involves analyzing and predicting the hazardous nature of Near-Earth Objects (NEOs) using historical data provided by NASA. The dataset includes various features such as absolute magnitude, estimated diameter, relative velocity, and miss distance. A Random Forest classifier is used to predict whether an NEO is hazardous based on these features.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Steps Taken](#steps-taken)
3. [Data Description](#data-description)
4. [Results](#results)

## Project Overview
This repository contains a machine learning model that predicts whether a Near-Earth Object is hazardous or not. The model is trained using a dataset that includes historical records of NEOs from 1910 to 2024. The primary goal is to provide a tool that can help in identifying potential threats from space.

## Steps Taken
1. **Data Collection**:
   - Gathered the NEO dataset from NASA's database, which includes records from 1910 to 2024.

2. **Data Preprocessing**:
   - Cleaned the dataset by handling missing values and removing irrelevant or duplicate entries.
   - Converted categorical variables to numerical format using encoding techniques.
   - Normalized features to ensure consistent scaling for the machine learning model.

3. **Exploratory Data Analysis (EDA)**:
   - Analyzed the dataset to understand the distribution of features and the relationship between variables.
   - Visualized data using plots to identify patterns and correlations.

4. **Feature Selection**:
   - Selected relevant features based on their importance and impact on the target variable (`is_hazardous`).

5. **Model Building**:
   - Split the dataset into training and test sets to evaluate model performance.
   - Trained a Random Forest classifier on the training set to predict hazardous NEOs.
   - Tuned hyperparameters to optimize the model's performance.

6. **Model Evaluation**:
   - Evaluated the model using metrics such as accuracy, confusion matrix, precision, recall, and F1-score.
   - Validated the model’s predictions on the test set to ensure robustness.

7. **Results Interpretation**:
   - Analyzed the model’s predictions and performance metrics to assess its effectiveness.
   - Generated visualizations to illustrate the model’s results and accuracy.

8. **Documentation**:
   - Documented the process, results, and findings in this `README.md` file for clarity and reproducibility.

## Data Description
The dataset is sourced from NASA and includes the following columns:
- `neo_id`: Unique identifier for each NEO.
- `name`: Name given by NASA.
- `absolute_magnitude`: Describes intrinsic luminosity.
- `estimated_diameter_min`: Minimum estimated diameter in kilometers.
- `estimated_diameter_max`: Maximum estimated diameter in kilometers.
- `relative_velocity`: Velocity relative to Earth in km/h.
- `miss_distance`: Distance in kilometers missed.
- `is_hazardous`: Boolean feature indicating whether the NEO is harmful.

The dataset contains 338,199 entries.

## Results
The Random Forest model achieved an accuracy of approximately 91.75% on the test dataset. The model's confusion matrix shows the following:

- True Negatives (TN): 56,993
- False Positives (FP): 2,018
- False Negatives (FN): 3,563
- True Positives (TP): 5,066

