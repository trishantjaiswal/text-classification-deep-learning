# Text Classification using Deep Learning

This repository contains a **step-by-step NLP project** that builds a text classification system, starting from traditional machine learning and designed to be extended to deep learning models.

---

## 📌 Problem Statement
Given a piece of text, classify it into one of several predefined categories using machine learning techniques.

---

## 📂 Dataset
- **Source**: 20 Newsgroups (scikit-learn)
- **Categories used**:
  - rec.autos
  - sci.med
  - comp.graphics
  - sci.space
- **Total samples**: ~3,900 documents

---

## 🧠 Approach

### 1. Data Preprocessing
- Removed headers, footers, and quoted text
- Train–test split (80% / 20%)

### 2. Feature Extraction
- TF-IDF Vectorization
- Maximum features: 5000
- English stopwords removed

### 3. Model
- Logistic Regression
- Solver optimized with increased max iterations

### 4. Evaluation
- Accuracy score
- Precision, Recall, F1-score (classification report)

---

## 📊 Results
- **Test Accuracy**: ~85–90%
- Strong baseline performance for a traditional ML model on text data

---

## 📁 Repository Structure
