# Diabetes Prediction using Machine Learning

This repository contains a machine learning project that predicts **diabetes presence** based on patient health indicators and symptoms.  
The project uses multiple supervised learning algorithms to analyze the dataset and compare performance across models.  

---

## Project Overview
Diabetes is one of the most prevalent chronic diseases worldwide. Early detection and prediction can help in proper medical management and prevention of complications.  

This project applies various **machine learning classifiers** to a clinical dataset (`diabetes_data_upload.csv`) to predict whether a patient is **Positive** or **Negative** for diabetes.  

---

## Methodology
1. **Dataset**
   - Source: `diabetes_data_upload.csv` (520 records, 17 attributes).  
   - Attributes include: Age, Gender, Polyuria, Polydipsia, sudden weight loss, weakness, Polyphagia, Genital thrush, visual blurring, Itching, Irritability, delayed healing, partial paresis, muscle stiffness, Alopecia, Obesity, and class (target).  

2. **Preprocessing**
   - Handling categorical variables with **Label Encoding**.  
   - Scaling numeric features (Age) using **MinMaxScaler**.  
   - Splitting dataset into training (80%) and testing (20%).  

3. **Models Implemented**
   - Logistic Regression  
   - Decision Tree Classifier  
   - Random Forest Classifier  
   - XGBoost Classifier  

4. **Evaluation Metrics**
   - Accuracy  
   - Precision  
   - Recall  
   - F1-Score  
   - Confusion Matrix  
   - ROC Curves  

---

## Results Highlights
- **Logistic Regression**  
  - Accuracy: **93.27%**  
  - F1 Score: **95.10%**  

- **Decision Tree**  
  - Accuracy: **95.19%**  
  - F1 Score: **96.35%**  

- **Random Forest (Best)**  
  - Accuracy: **99.04%**  
  - Precision: **100%**  
  - Recall: **98.59%**  
  - F1 Score: **99.29%**  

- **XGBoost**  
  - Accuracy: **97.12%**  
  - F1 Score: **97.84%**  

**Random Forest** consistently outperformed other models, both before and after hyperparameter tuning:contentReference[oaicite:0]{index=0}.  

---

## Hyperparameter Tuning
- **Random Forest**  
  - Best Params: `{n_estimators: 300, max_depth: None, min_samples_split: 2, min_samples_leaf: 1}`  
  - Accuracy: **99.04%**  

- **XGBoost**  
  - Best Params: `{n_estimators: 300, learning_rate: 0.2, max_depth: 5, subsample: 0.9}`  
  - Accuracy: **97.12%**  

---

## Repository Contents
- `Diabetes.ipynb - Colab.pdf` → Notebook with full analysis, modeling, and results.  
- `diabetes_data_upload.csv` → Dataset used for training and testing.  


