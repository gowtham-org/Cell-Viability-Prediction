# 📊 Cell Viability Prediction using Machine Learning

This project builds a machine learning pipeline to predict cell viability based on gene expression data using various regression models such as Random Forest, Ridge Regression, and XGBoost. The workflow involves preprocessing, feature scaling, model training, hyperparameter tuning, and evaluation.

---

## 🧪 Dataset Sources
Download dataset csv files from below URL
https://depmap.org/portal/data_page/?tab=allData
- **Gene Expression**: `OmicsExpressionProteinCodingGenesTPMLogp1BatchCorrected.csv`
- **Model Metadata**: `Model.csv`
- **Cell Viability**: `sanger-viability.csv`


---

## ✅ Steps Followed

1. **Mounted Google Drive** to access datasets within Google Colab.
2. **Loaded datasets**: gene expression data, metadata, and viability data using `pandas`.
3. **Merged datasets** on common identifiers for a unified analysis.
4. **Cleaned the data**:
   - Removed columns with more than 50% missing values.
   - Imputed missing values using median or categorical defaults.
5. **Scaled the features** using `StandardScaler` to normalize the input features.
6. **Split the dataset** into training and testing sets using `train_test_split`.
7. **Trained multiple models**:
   - `RandomForestRegressor`
   - `Ridge` Regression
   - `XGBRegressor`
8. **Performed Hyperparameter Tuning** using `GridSearchCV` to optimize model performance.
9. **Visualized Results**:
   - Feature importance plots
   - Prediction scatterplots
   - Correlation heatmaps
10. *(Optional)* Applied dimensionality reduction (e.g., PCA) to analyze feature space and reduce noise.

---

## 📈 Evaluation Metrics
- **Root Mean Squared Error (RMSE)**
- **R² Score**

---

## 📦 Dependencies
```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
