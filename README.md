House Price Prediction (Regression Project)
📌 Project Overview

This project is focused on building and comparing different regression models to predict house prices.
Since the dataset contains ~380 rows, the goal was to experiment with baseline linear models and tree-based ensemble methods, then evaluate their performance using cross-validation.

📂 Dataset

The dataset used for this project contains around 380 observations.

No separate test.csv file was provided.

Models were therefore evaluated using 5-Fold Cross-Validation to ensure stable and reliable performance estimates.

🛠️ Models Used

The following models were trained and evaluated:

Linear Regression (Baseline)

Random Forest Regressor

XGBoost Regressor

📊 Results
Model	Mean CV R²	Notes
Linear Regression	~0.72	Decent baseline but limited by linearity
Random Forest	0.78 ± 0.07	Best performing, stable, handled non-linearity well
XGBoost	~0.77–0.79	Performed close to RF, but slightly lower on this small dataset

✅ Random Forest was the final chosen model, as it consistently gave the best cross-validation performance.

🔑 Key Insights

Random Forest worked best because the dataset was small (380 rows) → boosting methods like XGBoost didn’t outperform RF.

Cross-validation was essential to avoid overfitting and to validate performance without a dedicated test set.

Tree-based methods significantly outperformed simple linear regression.

📌 Next Steps (Future Work)

Experiment with feature engineering (log-transform, interaction features).

Try stacking/ensembling RF + Linear + XGBoost for potential improvements.

Collect a larger dataset → boosting models like XGBoost/LightGBM may outperform RF with more data.

🏆 Final Takeaway

On small datasets (~380 rows), Random Forest is often the most reliable model, balancing bias and variance.
In this project, Random Forest achieved R² ≈ 0.78 ± 0.07 (cross-validated), making it the best choice.

Image link: 
