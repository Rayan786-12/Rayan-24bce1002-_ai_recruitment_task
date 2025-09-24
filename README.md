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
- Vectorization using **BoW, TF-IDF, W2V, and Doc2Vec**  

---

## 4. Models Implemented
1. Logistic Regression (BoW & TF-IDF)  
2. Linear SVM (TF-IDF)  
3. Random Forest (W2V)  
4. Naive Bayes (BoW, TF-IDF, W2V, Doc2Vec)  

---

## 5. Model Training
- Train/test split: 80/20  
- Default hyperparameters used for most models  
- Cross-validation applied where applicable  

---

## 6. Model Evaluation
- Metrics used: **Accuracy, Precision, Recall, F1-score**  
- Visualizations included:  
  - **Heatmaps** for confusion matrices  
  - **Histplots** for model comparison  
- Classification reports generated for all models  

| Model                       | Accuracy |
|------------------------------|---------|
| Logistic Regression (BoW)    | 0.8725  |
| Logistic Regression (TF-IDF) | 0.8857  |
| Linear SVM (TF-IDF)          | 0.8798  |
| Random Forest (W2V)          | 0.8327  |
| Naive Bayes (BoW)            | 0.8436  |
| Naive Bayes (TF-IDF)         | 0.8723  |
| Naive Bayes (W2V)            | 0.7611  |
| Naive Bayes (Doc2Vec)        | 0.7218  |

---

## 7. Observations
- **Best performing model:** Logistic Regression (TF-IDF) → 0.8857 accuracy  
- Linear SVM (TF-IDF) is close second → 0.8798  
- Models using **BoW and TF-IDF** consistently outperform W2V and Doc2Vec features  
- Naive Bayes performs worst on W2V and Doc2Vec, showing limitation with embedding-based features  
- Visualizations like **heatmaps and histplots** provide clear insights into performance and metric comparisons  
- XGBoost was tested but underperformed (~0.8269), likely due to feature choice  

---

## 8. Conclusion
- **TF-IDF with Logistic Regression or Linear SVM** is the recommended approach for this task  
- Using multiple models shows breadth of approach and comparison  
- Including **evaluation metrics, classification reports, heatmaps, and histplots** enhances interpretability  
- Optional improvements:  
  - Hyperparameter tuning  
  - Dimensionality reduction (TruncatedSVD)  
  - Deep learning models (LSTM, BERT) for potentially higher performance  

---

## 9. Instructions to Run
1. Open the notebook in **Google Colab** or **Jupyter Notebook**  
2. Install necessary packages:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib xgboost nltk gensim
