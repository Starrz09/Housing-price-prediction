

🏡 Housing Price Prediction – Advanced Regression Project

📌 Overview
This project tackles the classic machine learning challenge of predicting house prices using the Ames Housing Dataset. With 79 features describing various aspects of residential properties, the goal is to build a robust regression model that can accurately estimate sale prices based on property attributes.

🎯 Objectives
- Understand how different features influence house prices.
- Build a regression pipeline that handles both categorical and numerical data.
- Evaluate multiple models and select the best-performing one.
- Ensure the model is generalizable, interpretable, and ready for deployment.

🧰 Tech Stack
- Languages: Python
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, LightGBM, CatBoost, Optuna
- Tools: Google Colab, Jupyter Notebook

📂 Dataset
- Source: Kaggle - House Prices: Advanced Regression Techniques
- Features: 79 explanatory variables including lot size, year built, neighborhood, quality ratings, and more.


🚀 Usage
1. Load the dataset (train.csv and test.csv).
2. Run the notebook Housingpriceprediction.ipynb.
3. The final predictions are saved as submission.csv.l

🔍 Key Features
- Data Cleaning: Imputation strategies based on feature context (e.g., filling missing pool quality with "None").
- Feature Engineering: Derived features like TotalBathrooms, TotalSF, HouseAge, and material quality scores.
- Exploratory Data Analysis (EDA): Visual insights into price trends, feature correlations, and material impact.
- Modeling:
  - Ridge Regression (baseline)
  - Random Forest
  - XGBoost
  - LightGBM
  - CatBoost
- Hyperparameter Tuning: Grid search and Optuna optimization for LightGBM and CatBoost.
- Final Model: Tuned CatBoost Regressor with RMSE ≈ 0.1129.

📊 Model Performance Summary

| Model        | Training R² | CV Mean R² | CV RMSE |
|--------------|-------------|------------|---------|
| Ridge        | 0.9382      | 0.8754     | 0.1396  |
| RandomForest | 0.9821      | 0.8787     | 0.1388  |
| XGBoost      | 0.9996      | 0.8830     | 0.1363  |
| LightGBM     | 0.9900      | 0.8958     | 0.1286  |
| CatBoost     | 0.9808      | 0.9155     | 0.1129 |

📈 Feature Importance
Top features influencing price:
- QualSF
- OverallCond
- GrLivArea
- TotalSF
- Neighborhood_Category
- OverallQual
- KitchenQual

📤 Submission
- Predictions are log-transformed and inverse-transformed before submission.
- Final output: submission.csv with Id and SalePrice.

👤 Author
Lawal Habeeb
Pharmacist and Aspiring data scientist
GitHub: Starrz09
email: habeebobashola09@gmail.com
