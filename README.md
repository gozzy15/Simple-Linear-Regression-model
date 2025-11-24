# Simple-Linear-Regression-model

# Week 1 Machine Learning Project  
## Predicting Student Exam Performance Using Linear Regression

## Overview
This project explores the key factors that influence students’ exam performance. The goal was to analyze study-related behaviors, identify which factors most strongly impact exam scores, and build a simple predictive model using linear regression.

## Tools Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-Learn (sklearn)  
- Jupyter Notebook  

## Loading and Exploring the Dataset
The dataset includes the following variables:

- Hours Studied  
- Attendance Rate  
- Exam Score  

Initial exploration was performed using `df.info()` and `df.describe()` to understand the dataset structure, data types, and statistical summaries.

## Visualizing Relationships
Scatter plots were used to explore relationships between the variables and exam performance:

- Hours Studied vs Exam Score  
- Attendance Rate vs Exam Score  

### Insights
- Hours studied showed a strong positive correlation with exam scores.  
- Attendance rate showed a weaker but noticeable influence.

### Correlation Results
| Variable Pair | Correlation |
|---------------|-------------|
| Hours Studied vs Exam Score | 0.8146 |
| Attendance Rate vs Exam Score | 0.2177 |
| Hours Studied vs Attendance | -0.0874 |

Hours Studied was the strongest predictor, with a Pearson correlation of **0.8146** (p-value ≈ 1e-48), indicating a strong and statistically significant relationship.

## Building the Linear Regression Model
A linear regression model was created using:

- **Predictor (X):** Hours Studied  
- **Target (y):** Exam Score  

The regression line was plotted over the scatter data to visualize the model fit.

The dataset was split using `train_test_split()`:

- 80% training data  
- 20% testing data  
- `random_state=42` for reproducibility  

## Model Evaluation
A custom evaluation function calculated the following metrics:

- R-squared (R²)  
- Mean Absolute Error (MAE)  
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  

### Training Performance
- R²: 0.6593  
- MAE: 4.6463  
- MSE: 34.2023  
- RMSE: 5.8483  

### Testing Performance
- R²: 0.6753  
- MAE: 4.7044  
- MSE: 35.1104  
- RMSE: 5.9254  

The similar training and testing results indicate that the model generalizes well.  
Study hours remain a strong and reliable predictor of exam performance.

## What I Learned
- How to inspect and clean datasets using Pandas  
- How to visualize relationships with Matplotlib  
- How to interpret correlation using Pearson’s coefficient  
- How to build and evaluate a Linear Regression model  
- How to calculate R², MAE, MSE, and RMSE  
- Why study hours strongly predict academic performance  
