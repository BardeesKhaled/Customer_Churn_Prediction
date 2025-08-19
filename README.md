# Customer Churn Prediction 📊

## 📌 Project Overview
This project focuses on **predicting customer churn** using machine learning models. Customer churn (also known as customer attrition) is when customers stop doing business with a company. By predicting churn, businesses can take proactive measures to retain valuable customers.  

The project explores different machine learning algorithms, compares their performance, and identifies the best model for churn prediction.

---

## 📂 Dataset
The dataset used contains customer information such as:
- Demographics (e.g., gender, age)
- Services subscribed
- Contract and billing details
- Churn status (target variable)

---

## ⚙️ Models Trained
The following models were trained and evaluated using **GridSearchCV** with cross-validation:

1. **Random Forest Classifier**  
2. **Logistic Regression**  
3. **Naive Bayes (GaussianNB)**  
4. **Decision Tree Classifier**  
5. **XGBoost Classifier**

---

## 📊 Results
| Model                | Best Score | Best Parameters          |
|-----------------------|------------|--------------------------|
| Random Forest         | 0.7854     | {'n_estimators': 10}     |
| Logistic Regression   | 0.7927     | {'C': 1}                 |
| Naive Bayes           | 0.3745     | {}                       |
| Decision Tree         | 0.7941     | {'criterion': 'gini'}    |
| XGBoost Classifier    | **0.8219** | {'base_score': 0.5}      |

✅ **XGBoost achieved the highest accuracy (82.19%)**, making it the best performing model for this dataset.

---

## 🚀 Tech Stack
- **Python**
- **Pandas, NumPy** (Data preprocessing)
- **Matplotlib, Seaborn** (Visualization)
- **Scikit-learn** (ML models, GridSearchCV)
- **XGBoost** (Boosting algorithm)
- **Jupyter Notebook**

---

## 📈 How It Works
1. Data preprocessing (handling missing values, encoding categorical variables, scaling features).
2. Splitting dataset into training and testing sets.
3. Training multiple machine learning models.
4. Hyperparameter tuning using **GridSearchCV**.
5. Evaluating performance and selecting the best model.
6. Comparing results of all models.

---

## 📌 Key Takeaways
- Logistic Regression and Decision Tree performed fairly well.  
- Naive Bayes struggled due to dataset complexity and feature interactions.  
- XGBoost outperformed all with **82% accuracy**, proving its strength in handling churn prediction tasks.

---

## 💡 Future Improvements
- Try advanced feature engineering.  
- Implement deep learning models (e.g., LSTMs for time-series churn prediction).  
- Deploy the best model using **Flask/RestAPI** for real-world usage.  

---
