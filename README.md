# 🌍 Climate Misinformation Detection using NLP

---

## 📌 Project Overview

This project builds a **Natural Language Processing (NLP)** system to detect climate-related misinformation.  
It classifies climate claims into:

- ✅ **SUPPORTS (True Claim)**
- ❌ **REFUTES (False / Misleading Claim)**

The model is trained on the **Climate-FEVER dataset** and implements text preprocessing, feature extraction, machine learning classification, and evaluation techniques.

---

## 🎯 Objective

To build a **binary classification model** that can automatically verify climate-related claims and detect misinformation using NLP techniques.

---

## 📂 Dataset

- **Dataset:** Climate-FEVER  
- Contains climate-related claims with verification labels  

### Original Labels:
- SUPPORTS  
- REFUTES  
- NOT_ENOUGH_INFO  

### For this project:
- Converted into **Binary Classification**
- Removed `NOT_ENOUGH_INFO`

---

## ⚙️ Project Pipeline

### 1️⃣ Data Preprocessing

The following NLP techniques were applied:

- URL removal  
- Hashtag & mention removal  
- Emoji removal  
- Lowercasing  
- Tokenization  
- Stopword removal  
- Lemmatization  

This ensures clean and normalized text for modeling.

---

### 2️⃣ Exploratory Data Analysis (EDA)

Performed:

- Word frequency distribution  
- Word cloud visualization  
- Analysis of frequent climate-related terms  

This helped understand textual patterns in climate claims.

---

### 3️⃣ Feature Engineering

Used **TF-IDF (Term Frequency – Inverse Document Frequency)** to convert textual data into numerical vectors suitable for machine learning.

---

### 4️⃣ Model Building

Implemented:

- Logistic Regression Classifier  
- Applied `class_weight='balanced'` to handle class imbalance  

---

### 5️⃣ Model Evaluation

Evaluated using:

- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  
- ROC Curve  
- AUC Score  

---

## 📊 Final Model Performance

- **Accuracy:** ~69%  
- **AUC Score:** 0.68  
- Improved minority class recall using class balancing  

The model demonstrates moderate ability to distinguish between true and misleading climate claims.

---

## 📈 Key Insights

- Dataset was imbalanced (more SUPPORTS than REFUTES)  
- Accuracy alone was misleading  
- Applying class balancing significantly improved detection of misleading claims  
- Feature importance revealed key words influencing predictions  

---

## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- NLTK  
- spaCy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 🚀 Future Improvements

- Implement Transformer models (BERT)  
- Hyperparameter tuning  
- Cross-validation  
- Advanced imbalance handling (SMOTE)  
- Model deployment using Flask or Streamlit  

---

## 💾 Project Structure
