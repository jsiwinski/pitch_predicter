# Pitch Type Classification

This project builds a machine learning model to predict the next pitch type in a baseball game using pitch-by-pitch data from the 2011 MLB season.

## Workflow

- **Data Loading & Cleaning:** Loaded pitch-level and metadata CSVs, removed columns with excessive missing data, handled missing values, and checked for duplicates.
- **Exploratory Data Analysis (EDA):** Explored class imbalance, feature distributions, and relationships between features and pitch type.
- **Feature Engineering:** Created contextual and sequential features, including pitcher-specific pitch usage, previous pitch types, count leverage, and pitch streaks.
- **Model Training:** Compared multinomial logistic regression (with class weighting) and XGBoost (with SMOTE oversampling and hyperparameter tuning) to address class imbalance.
- **Evaluation:** Assessed models using accuracy, macro F1-score, confusion matrices, ROC curves, and SHAP value analysis for interpretability.
- **Error Analysis:** Investigated confident model errors and low-confidence correct predictions to guide future improvements.
- **Future Steps:** Outlined ideas for advanced feature engineering, additional algorithms, better class imbalance handling, and real-world deployment.

## Key Results

- XGBoost with engineered features and SMOTE outperformed logistic regression, achieving strong accuracy and balanced performance across pitch types.
- Feature importance and SHAP analysis highlighted the value of pitcher arsenal metrics and sequential context.

## Next Steps

- Engineer first-pitch tendencies by pitcher
- Incorporate batter context and matchup data
- Explore additional models and ensemble methods
- Prepare for real-time deployment and further validation

---
