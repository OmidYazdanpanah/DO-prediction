# DO-prediction
This repository contains a complete machine-learning workflow for modeling **dissolved oxygen (DO)** from a set of water-quality / environmental predictors.
The script:
- Cleans and preprocesses the raw Excel data
- Explores correlations and pairwise relations between variables
- Trains and tunes three tree-based regressors (XGBoost, HistGradientBoosting, Random Forest) using `GridSearchCV`
- Selects the **best model based on MAE**
- Computes and visualizes **feature importance** using:
  - Built-in model importance (`feature_importances_`)
  - **Permutation importance** (more robust)
- Prints sample predictions and errors for a quick sanity check

> Dataset file used: **`DO_5DayAverage.xlsx`**  
> Target variable: **DO (mg/L)**
