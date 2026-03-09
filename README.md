# 🚗 Used Car Price Prediction using Machine Learning

## 📌 Project Overview

This project aims to predict the selling price of used cars using machine learning techniques. Accurate price prediction can help buyers, sellers, and online marketplaces make better pricing decisions.

The project explores the relationship between vehicle characteristics (such as brand, engine capacity, mileage, and power) and their impact on resale value.

Three tree-based regression models were trained and evaluated to identify the most accurate approach for price prediction.

---

# 📊 Dataset

The dataset contains various features describing used vehicles, including:

- Brand
- Engine capacity
- Mileage
- Transmission type
- Torque
- Max power
- Manufacturing year
- Seller type

The target variable is:

**Selling Price**

---

# 🛠 Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**

Machine Learning Models:

- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

---

# 🔎 Exploratory Data Analysis (EDA)

Several exploratory analyses were conducted to understand the dataset.

Key steps included:

- Handling missing values
- Visualizing feature distributions
- Identifying correlations between variables

### Feature Correlation with Car Price

The heatmap below highlights the **top features most strongly correlated with selling price**.

<img width="1133" height="688" alt="Correlation Heatmap" src="https://github.com/user-attachments/assets/660c2c0b-95d5-4212-afc5-bcf4bf94bb8f" />

Key observations:

- **Max Power** and **Engine Capacity** have strong positive correlations with selling price.
- Premium brands such as **BMW** also show higher price associations.
- Manual transmission tends to correlate negatively with price.

---

# 🤖 Model Training & Evaluation

Three regression models were trained using **5-fold cross-validation** to ensure robust performance evaluation.

### Model Performance (Before Feature Selection)

| Model | Mean R² | Standard Deviation |
|------|------|------|
| Decision Tree | 0.9006 | 0.0435 |
| Random Forest | **0.9304** | 0.0365 |
| Gradient Boosting | 0.9053 | 0.0282 |

Random Forest achieved the highest predictive performance among the tested models.

---

# 📉 Feature Selection (Dimensionality Reduction)

To improve efficiency and reduce noise in the dataset, **feature selection** was performed using the Random Forest feature importance scores.

Method used:

**SelectFromModel (median threshold)**

This removed less informative features while retaining the most impactful predictors.

### Model Performance After Feature Selection

| Model | Mean R² | Standard Deviation |
|------|------|------|
| Decision Tree | 0.902 | 0.0451 |
| Random Forest | **0.9308** | 0.0359 |
| Gradient Boosting | 0.9039 | 0.0291 |

The results show that **dimensionality reduction maintained model performance while simplifying the feature space.**

---

# 📈 Key Insights

Important findings from the analysis include:

- Vehicle **power and engine size** are strong predictors of price.
- **Premium brands** significantly influence resale value.
- Feature selection helped **reduce model complexity without sacrificing accuracy**.
- Random Forest consistently delivered the **best predictive performance**.
