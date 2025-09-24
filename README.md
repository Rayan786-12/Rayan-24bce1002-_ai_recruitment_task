# Rayan-24bce1002-_ai_recruitment_task
# IMDb Movie Review Sentiment Analysis

## Student Information
- **Name:** Rayan Ahmed
- **ID:** 24BCE1002
- **Task:** AI/ML Recruitment Task

---

## 1. Project Overview
This project performs **sentiment analysis** on IMDb movie reviews.  
The goal is to classify reviews as **Positive** or **Negative** using multiple machine learning models and compare their performance.

---

## 2. Dataset
- **Source:** IMDb Movie Review Dataset  
- **Size:** 50,000 reviews (balanced Positive and Negative)  
- **Format:** CSV with columns `review` and `sentiment`  

---

## 3. Data Preprocessing
- Text cleaning: removing punctuation, lowercasing  
- Tokenization  
- Stopwords removal  
- Lemmatization  
- Vectorization using **CountVectorizer** and **TF-IDF**

---

## 4. Models Implemented
1. Logistic Regression  
2. Support Vector Machine (SVM)  
3. Random Forest  
4. XGBoost  

---

## 5. Model Training
- Train/test split: 80/20  
- Hyperparameter tuning using default parameters or GridSearchCV  
- Cross-validation applied where necessary  

---

## 6. Model Evaluation
- Metrics: Accuracy, Precision, Recall, F1-score  
- Confusion matrix for each model  
- Classification report for each model  
- Performance comparison across all models  

---

## 7. Results
- **Best performing model:** XGBoost  
- **Overall accuracy:** ~0.90  
- Confusion matrices and bar charts of Precision, Recall, F1-score included in the notebook  

---

## 8. Observations
- XGBoost achieves the highest accuracy and balanced class performance  
- Logistic Regression and SVM perform slightly lower but are still competitive  
- Random Forest handles class imbalance better than others  
- Insights can guide future improvements in feature engineering and hyperparameter tuning  

---

## 9. Conclusion
- Multiple ML models can successfully classify IMDb reviews  
- XGBoost is recommended for this dataset based on metrics  
- Future work: Incorporate deep learning models (LSTM/BERT) for potentially higher performance  

---

## 10. Instructions to Run
1. Open the notebook in **Google Colab** or **Jupyter Notebook**  
2. Install necessary packages:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib xgboost nltk
