# 📝 Text Classification using Machine Learning & Deep Learning

This repository demonstrates a **complete Natural Language Processing (NLP) pipeline** for text classification, progressing from a **traditional machine learning baseline** to a **deep learning model built with TensorFlow and Keras**.

The project is designed to be **educational, extensible, and presentation-ready**, making it suitable for learning, interviews, and portfolio showcasing.

---

## 📌 Problem Statement

Given a piece of text, the task is to **classify it into one of several predefined categories** using supervised learning techniques.

---

## 📂 Dataset

- **Dataset**: 20 Newsgroups (via scikit-learn)
- **Selected Categories**:
  - `rec.autos`
  - `sci.med`
  - `comp.graphics`
  - `sci.space`
- **Total Samples**: ~3,940 documents
- **Preprocessing**:
  - Removed headers, footers, and quoted text
  - Used cleaned raw text for modeling

---

## 🧠 Project Overview

This project is implemented in **two stages** to clearly compare traditional NLP methods with deep learning approaches.

---

## 1️⃣ TF-IDF + Logistic Regression (Baseline)

📓 **Notebook**: `01_tfidf_logistic_regression.ipynb`

### Methodology
- **Text Representation**: TF-IDF Vectorization  
  - Max features: 5000  
  - English stopwords removed
- **Model**: Logistic Regression
- **Train–Test Split**: 80% / 20%

### Evaluation
- Accuracy
- Precision, Recall, F1-score

### Results
- **Test Accuracy**: ~88%
- Strong, interpretable baseline with minimal computation

---

## 2️⃣ Deep Learning with TensorFlow & Keras

📓 **Notebook**: `02_tensorflow_text_classification.ipynb`

This notebook replaces manual feature engineering with **learned word embeddings** and a neural network architecture.

### Model Architecture
- TextVectorization layer
- Embedding layer
- Global Average Pooling
- Dense hidden layer (ReLU)
- Softmax output layer

### Training Details
- **Framework**: TensorFlow & Keras
- **Loss Function**: Sparse Categorical Crossentropy
- **Optimizer**: Adam
- **Epochs**: 10
- **Batch Size**: 32
- **Validation Split**: 20%

### Results
- **Validation Accuracy**: ~81–85%
- **Test Accuracy**: ~81%
- Demonstrates semantic learning and scalability

---

## 📊 Model Comparison

| Model | Feature Type | Test Accuracy |
|------|-------------|---------------|
| TF-IDF + Logistic Regression | Sparse statistical features | ~88% |
| TensorFlow Neural Network | Learned embeddings | ~81% |

---

## 📁 Repository Structure

