# Fake News Prediction Using Logistic Regression

This machine learning project is centered on detecting fake news articles using logistic regression. The dataset consists of news-related metadata, and the objective is to classify news as real (`0`) or fake (`1`). Extensive text preprocessing was carried out before modeling, and classification metrics were used to evaluate the model's performance.

---

## Project Objective  
To build a classification model that can accurately distinguish between real and fake news based on textual features extracted from author names and titles.

---

## What Was Done  
- Loaded and explored the dataset, handling missing values with `dropna()`.
- Merged **author** and **title** columns into a single **content** field for more contextual textual analysis.
- Applied comprehensive text preprocessing:
  - Lowercasing
  - Removal of punctuation and non-alphabetic characters
  - Stopword removal
  - Stemming using `PorterStemmer`
- Converted text into numeric format using **TF-IDF Vectorization**.
- Split data with a **test size of 20%**.
- Trained a **Logistic Regression** model.
- Evaluated model performance using:
  - **Confusion Matrix**
  - **Classification Report**
  - **ROC Curve**
  - **Precision-Recall Curve**
  - **Classification Metrics Bar Plot**
  - **Log Loss Curve**
  - **Feature Importance Plot**
  - **Learning Curve**

---

## Classification Model Evaluation

### Training Data

| Metric        | Score   |
|---------------|---------|
| **Accuracy**  | 0.990   |
| **Precision** | 0.985   |
| **Recall**    | 0.993   |
| **F1 Score**  | 0.989   |

### Testing Data

| Metric        | Score   |
|---------------|---------|
| **Accuracy**  | 0.982   |
| **Precision** | 0.969   |
| **Recall**    | 0.991   |
| **F1 Score**  | 0.980   |

---

## Summary of Key Insights
- The model demonstrated **high accuracy and generalization** with minimal overfitting, evidenced by similar performance on training and testing data.
- **TF-IDF Vectorization** was effective for transforming text into numerical features suitable for logistic regression.
- Most fake news articles were correctly identified, showing **high recall** on both training and testing sets.
- The **confusion matrix** revealed a low number of false positives and false negatives.
- **Feature importance plot** helped in understanding which words contributed most to the prediction.
- The **log loss and learning curves** showed the model converging well without signs of underfitting or overfitting.

---

## Conclusion
- **Logistic Regression** provided a strong baseline for fake news detection, achieving high precision and recall.
- The model can be confidently used for binary news classification on similar datasets with minimal preprocessing.

---

**Developed by:** *Nischal Baidar*
