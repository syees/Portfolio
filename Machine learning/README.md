# Machine Learning Models Evaluation (R)

## Overview
This coursework applies multiple machine learning techniques to three datasets, covering **unsupervised learning, regression, and classification**.  
The goal is to demonstrate model development, evaluation, and comparison using R.

---

## Unsupervised Learning – Marketing Campaign
- **Dataset:** Marketing Campaign (Kaggle)  
- **Techniques:** Data cleaning, feature engineering, PCA, K-means clustering  
- **Key Insights:**
  - Cluster 1: Users with **lower purchasing power** (accepted fewer campaigns, lower spending)  
  - Cluster 2: Users with **higher purchasing power** (higher spending, higher purchases, more balanced income distribution)  

---

## Regression – House Sales Prediction
- **Dataset:** King County House Sales (Kaggle)  
- **Models Tested:** Linear Regression, Ridge, CART, Random Forest  
- **Results:**
  - Linear Regression: R² = 0.68 (overfitting issues)  
  - Random Forest: **Lowest RMSE**, best predictive performance for house prices  

---

## Classification – Stroke Prediction
- **Dataset:** Stroke Prediction (Kaggle)  
- **Models Tested:** Logistic Regression, LDA, KNN, Random Forest  
- **Results:**
  - Logistic Regression: Accuracy ~85%  
  - LDA: Accuracy 94.8%  
  - KNN: Accuracy 94.7%  
  - Random Forest: **Best accuracy 95.7%**  

---

## Key Takeaways
- **Clustering** revealed two distinct customer groups with different purchasing power  
- **Random Forest** consistently outperformed other models in regression & classification tasks  
- Feature engineering and proper handling of outliers were critical for better results  

