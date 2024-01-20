# Code Summary

## Data Preprocessing

- Imported necessary libraries (pandas, numpy, matplotlib, seaborn).
- Loaded and inspected the dataset ('laptop_data.csv').
- Removed the 'Unnamed: 0' column and handled missing values.
- Processed and converted columns 'Ram', 'Weight', 'X_res', 'Y_res', 'Memory', and 'HDD' for analysis.
- Extracted information from the 'ScreenResolution' column, creating new features.
- Processed and categorized the 'Cpu' and 'Gpu' columns.
- Transformed and categorized the 'Memory' column into storage layers and capacities.
- Processed the 'OpSys' column, categorizing it into 'Windows,' 'Mac,' and 'Others/No OS/Linux.'

## Data Visualization

- Visualized data using various plots, including histograms, bar plots, and scatter plots.

## Machine Learning

- Split the dataset into features (X) and the target variable (y).
- Applied one-hot encoding to categorical features using ColumnTransformer.
- Split the dataset into training and testing sets.
- Implemented several regression algorithms:
  - Linear Regression
  - Random Forest Regressor (Chosen Algorithm)
  - Ridge Regression
  - Lasso Regression
  - K-Nearest Neighbors Regressor
  - Decision Tree Regressor
  - Support Vector Machine Regressor (SVM)
  - Gradient Boosting Regressor
  - XGBoost Regressor
  - AdaBoost Regressor
  - Voting Regressor (Ensemble of Random Forest, Gradient Boosting, XGBoost, and Extra Trees)
  - Stacking Regressor (Ensemble of Random Forest, Gradient Boosting, and XGBoost with Ridge as the final estimator)

## Model Evaluation

- Evaluated each model's performance using R2 score and Mean Absolute Error (MAE).
- Saved the Random Forest Regressor model ('pipe.pkl') and the processed dataset ('df.pkl') using pickle.

## Conclusion

- The Random Forest Regressor yielded the best performance, as evidenced by the highest R2 score and the lowest MAE among the tested algorithms. Therefore, it was chosen as the final model for predicting laptop prices.
