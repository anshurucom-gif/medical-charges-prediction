# Medical Charges Prediction Using Linear Regression

## Project Overview

This project uses Python and Linear Regression to predict annual medical charges based on demographic, health, healthcare-utilization, and financial characteristics.

The project demonstrates a complete supervised machine-learning regression workflow, from exploratory data analysis and preprocessing to model evaluation and prediction.

## Business Problem

Healthcare costs can vary significantly between individuals. The objective of this project is to develop a regression model that can estimate annual medical charges based on available individual-level characteristics.

## Objective

Build and evaluate a Linear Regression model for predicting annual medical charges and use the trained model to generate a prediction for a hypothetical individual.

## Dataset

The dataset contains **1,338 observations** and includes 12 predictor variables along with the target variable `charges`.

### Features

* Age
* Sex
* BMI
* Number of children
* Smoker status
* Claim amount
* Past consultations
* Number of steps
* Hospital expenditure
* Number of past hospitalizations
* Annual salary
* Region

### Target Variable

`charges` — annual medical charges.

## Methodology

The project follows these steps:

1. Data loading and understanding
2. Exploratory Data Analysis
3. Data quality checks
4. Missing-value treatment
5. Outlier analysis
6. Categorical variable encoding
7. Train-test split
8. Linear Regression model development
9. Model evaluation
10. Residual and prediction-error analysis
11. Prediction for a hypothetical individual

## Model

The model used in this project is **Linear Regression**.

The dataset was divided into training and testing sets, with the test set used to evaluate the model's performance on unseen observations.

## Model Performance

| Metric | Result |
| ------ | -----: |
| R²     | 0.9632 |
| MAE    | 624.12 |
| RMSE   | 860.92 |

The model achieved an R² of **0.9632**, meaning that approximately 96.3% of the variation in medical charges was explained by the included features on the held-out test dataset.

The MAE was **624.12**, while the RMSE was **860.92**, indicating that the model performed well overall but had larger errors for some individual observations.

## Example Prediction

The trained model was used to predict annual medical charges for a hypothetical individual.

**Predicted annual medical charges: 7,095.64**

This represents a model estimate and should not be interpreted as an exact future medical cost.

## Key Findings

* The dataset contains substantial variation in annual medical charges.
* Several variables showed skewness and potential outliers during exploratory analysis.
* Extreme observations were investigated rather than automatically removed because they may represent legitimate observations.
* Linear Regression produced a strong R² on the held-out test data.
* Error analysis showed that the model both overpredicted and underpredicted charges for different observations.

## Limitations

* This project focuses on Linear Regression and does not compare multiple machine-learning algorithms.
* Missing numerical values were handled using median imputation.
* Categorical variables were numerically encoded.
* Model performance was evaluated using a single train-test split.
* Some variables may need further consideration regarding when the information becomes available in a real-world prediction scenario.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab
* GitHub

## Future Improvements

Future versions of this project could explore:

* Cross-validation
* Alternative encoding techniques
* Feature engineering
* Regularized regression models
* Tree-based regression models
* Model comparison and hyperparameter tuning

## Author

**Anshul Choudhary**
