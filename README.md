# 🏡 Boston Housing Price Prediction

## 📌 Problem Statement

The goal of this project is to predict housing prices for towns or suburbs in the Boston area using historical and environmental data. By identifying the most influential factors affecting housing prices, we aim to build an interpretable regression model and validate the assumptions underlying linear regression.

## 🎯 Objective

Build a linear regression model that:
- Accurately predicts housing prices (`MEDV`)
- Validates key linear regression assumptions (linearity, normality, homoscedasticity)
- Identifies statistically significant predictors

## 📊 Dataset

- **File**: `boston.csv`
- **Target Variable**: `MEDV` – Median value of owner-occupied homes in $1000s
- **Feature Attributes**:
  - `CRIM`: per capita crime rate by town
  - `ZN`: proportion of residential land zoned for lots over 25,000 sq. ft.
  - `INDUS`: proportion of non-retail business acres per town
  - `CHAS`: Charles River dummy variable (= 1 if tract bounds river)
  - `NOX`: nitric oxide concentration (parts per 10 million)
  - `RM`: average number of rooms per dwelling
  - `AGE`: proportion of owner-occupied units built before 1940
  - `DIS`: weighted distances to five employment centers
  - `RAD`: accessibility to radial highways
  - `TAX`: property-tax rate per $10,000
  - `PTRATIO`: pupil-teacher ratio
  - `LSTAT`: percentage of lower status population

## 📁 Repository Structure

```
├── SLF_W2_PracticeExercise_Solution.ipynb    # Notebook with data analysis and model
├── boston.csv                                # Dataset
├── README.md                                 # Project overview
```

## 🧪 Project Workflow

1. **Data Exploration & Cleaning**
   - Checked for nulls and outliers
   - Explored distribution of features and target variable

2. **Feature Analysis**
   - Visualized correlations using heatmaps
   - Explored feature relationships using pair plots

3. **Model Building**
   - Used `statsmodels` OLS for regression analysis
   - Verified statistical significance using p-values
   - Checked assumptions: linearity, normality of residuals, multicollinearity (VIF), and homoscedasticity

4. **Evaluation**
   - R² Score
   - Adjusted R²
   - Residual plots for model diagnostics

## 🏆 Results

- **Key Predictors**:
  - `RM`: number of rooms (positive influence)
  - `LSTAT`: % lower status population (negative influence)
  - `PTRATIO`: student-teacher ratio (negative influence)
- **Model Validity**:
  - R² ~ 0.73+
  - Model satisfies most key regression assumptions

## 🔍 Key Takeaways

- Linear regression remains a powerful baseline for structured tabular data
- Understanding statistical assumptions is crucial for interpretability
- Features like number of rooms and socio-economic indicators are strong drivers of housing prices

## 🚀 Future Enhancements

- Include polynomial terms for non-linear relationships
- Try regularized regressions (Ridge, Lasso)
- Deploy as a Flask app for user inputs and predictions

## 👨‍💻 Author

**Suhaib Khalid**  
Data Enthusiast | Statistical Modeler | Real Estate Analytics Explorer
