# Diamond Price Prediction Pipeline | ML Engineering Project

## Overview

Developed a production-ready machine learning pipeline to predict diamond prices using structured physical and categorical features. The project demonstrates core ML engineering practices including data validation, feature engineering, automated preprocessing, model training, evaluation, and interpretability.

Model performance:

- R² Score: 0.9811  
- Mean Absolute Error: $206  

---

## ML Engineering Highlights

- Built an end-to-end Pipeline using Scikit-learn to automate preprocessing and training
- Used ColumnTransformer to handle mixed numerical and categorical features
- Implemented feature engineering by creating a volume feature (`volume = x * y * z`)
- Applied IQR-based outlier removal to improve model generalization
- Prevented data leakage through proper Pipeline-based architecture
- Designed workflow to be reproducible and deployment-ready

---

## Pipeline Architecture
Input Data
→ ColumnTransformer
├── StandardScaler (numerical features)
└── OneHotEncoder (categorical features)
→ RandomForestRegressor
→ Prediction Output

This modular design enables seamless integration into production systems, APIs, or real-time ML applications.

---

## Model and Evaluation

Model: Random Forest Regressor

Results:

- Explains 98.11% of price variance
- Low prediction error ($206 MAE)
- Residual analysis confirms unbiased predictions

Top predictive features: carat, volume, clarity, and physical dimensions.

---

## Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## Deployment Readiness

The Pipeline architecture ensures:

- Reproducible training and inference
- Easy model serialization (joblib / pickle)
- Compatibility with web apps, ML APIs, and production systems

---

## Author

Vertika Singh  
B.Tech Computer Science  
Machine Learning and Artificial Intelligence
