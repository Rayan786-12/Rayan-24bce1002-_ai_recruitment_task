# IMDb Movie Review Sentiment Analysis

## Student Information
- **Name:** Rayan Ahmed
- **ID:** 24BCE1002
- **Task:** AI/ML Recruitment Task

---

## Project Overview
This project performs **binary sentiment analysis** on IMDb movie reviews.  
The goal is to classify reviews as **Positive** or **Negative** using multiple machine learning models and compare their performance.

---

## Approach
1. **Data Preprocessing**
   - Text cleaning, lowercasing, tokenization  
   - Stopwords removal and lemmatization  
   - Vectorization: **BoW, TF-IDF, Word2Vec, Doc2Vec**

2. **Models Used**
   - Logistic Regression (BoW & TF-IDF)  
   - Linear SVM (TF-IDF)  
   - Random Forest (W2V)  
   - Naive Bayes (BoW, TF-IDF, W2V, Doc2Vec)

3. **Evaluation**
   - Metrics: **Accuracy, Precision, Recall, F1-score**  
   - Visualizations: **Heatmaps** for confusion matrices, **Histplots** for model comparison  
   - Classification reports generated for all models

---

## Key Results
| Model                       | Accuracy |
|------------------------------|---------|
| Logistic Regression (TF-IDF) | 0.8857  |
| Linear SVM (TF-IDF)          | 0.8798  |
| Random Forest (W2V)          | 0.8327  |
| Naive Bayes (TF-IDF)         | 0.8723  |

- **Best Model:** Logistic Regression with TF-IDF  
- XGBoost tested (~0.8269) but TF-IDF models performed better  
- Visualizations and metrics provide clear comparison between models

---

## Conclusion
- **Recommended approach:** TF-IDF vectorization + Logistic Regression or Linear SVM  
- Using multiple models and visualization enhances interpretability and robustness
