# 🚗 Used Car Price Prediction: Machine Learning Approach

## 🛠 Tech Stack
- Language: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Machine Learning**: Decision Tree, Random Forest Regressor, Gradient Boosting Regressor
  
<img width="1133" height="688" alt="Screenshot 2026-03-06 214436" src="https://github.com/user-attachments/assets/660c2c0b-95d5-4212-afc5-bcf4bf94bb8f" />

## 🚀 Key Workflows

1. **Exploratory Data Analysis (EDA) & Preprocessing**
- Handled missing values to ensure data integrity.
- Visualized feature distributions (e.g., fuel types, top car brands) and analyzed the correlation matrix to identify key price drivers.
- Applied One-Hot Encoding for categorical variables (e.g., Brand, Fuel Type) to prepare data for non-linear models.

2. **Modeling & Evaluation**
- Trained and evaluated three tree-based regression models using 5-fold Cross-Validation to prevent overfitting.
- Random Forest and Gradient Boosting outperformed the basic Decision Tree, capturing complex non-linear relationships in the pricing data.

3. **Dimensionality Reduction (Feature Selection)**
- Extracted Feature Importances using the Random Forest model.
- Applied SelectFromModel (using the median threshold) to filter out noise and retain only the most impactful features.
- Impact: Successfully reduced data dimensionality while maintaining high predictive accuracy, optimizing the model for faster deployment.
          <img width="699" height="707" alt="Screenshot 2026-03-06 214455" src="https://github.com/user-attachments/assets/b50547dd-3889-4f4d-b389-5e7c300f85c4" />

