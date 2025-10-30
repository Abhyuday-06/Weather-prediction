# Weather Prediction Using Linear Regression

This project implements linear regression from scratch to predict weather patterns using historical weather data.

## Project Overview

The repository contains two main implementations:

1. **Simple_Linear_Regression.ipynb** - Basic linear regression for weather classification
2. **Multivariate_Linear_Regression.ipynb** - Multivariate linear regression with feature normalization for temperature prediction

## Features

- Custom implementation of gradient descent algorithm
- Feature normalization for better convergence
- Cost function visualization
- Prediction evaluation with error metrics
- Data preprocessing and encoding for categorical variables

## Dataset

The project uses `weatherHistory.csv` which contains various weather parameters:
- Temperature (C)
- Humidity
- Visibility (km)
- Pressure (millibars)
- Cloud Cover
- Wind Speed (km/h)
- Precip Type
- Summary
- Daily Summary

## Requirements

Install the required packages using:

```bash
pip install -r requirements.txt
```

## Usage

1. Ensure `weatherHistory.csv` is in the project directory
2. Open the desired Jupyter notebook
3. Run all cells sequentially

### Simple Linear Regression
```bash
jupyter notebook "Simple_Linear_Regression.ipynb"
```

### Multivariate Linear Regression
```bash
jupyter notebook "Multivariate_Linear_Regression.ipynb"
```

## Implementation Details

### Gradient Descent
The algorithm minimizes the cost function by iteratively updating theta parameters:
- **Learning rate (α)**: Controls the step size
- **Iterations**: Number of updates to perform
- **Update rule**: θ = θ - (α/m) × X^T(Xθ - y)

### Feature Normalization
Applied in the multivariate model to ensure all features are on similar scales:
- Formula: (value - mean) / (max - min)
- Helps gradient descent converge faster

### Cost Function
Measures prediction accuracy using Mean Squared Error:
- J(θ) = (1/2m) × Σ(prediction - actual)²
- Lower cost indicates better model performance

## Results

The models track cost reduction across iterations and evaluate predictions using:
- Root Mean Square Error (RMSE)
- Visual cost convergence plots
- Actual vs predicted value comparisons

