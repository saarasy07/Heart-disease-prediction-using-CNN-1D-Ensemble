# 🧠 Heart Arrhythmia Classification using Ensemble 1D CNN with SMOTEENN

## 📌 Overview

Cardiac arrhythmia is a condition characterized by irregular heart rhythms and can lead to serious health complications if not detected early. Electrocardiogram (ECG) signals provide essential information for identifying such abnormalities.

This project proposes a deep learning-based classification system using an **Ensemble One-Dimensional Convolutional Neural Network (1D CNN)** combined with **SMOTEENN resampling** to handle class imbalance in ECG data. The ensemble approach integrates multiple CNN models with different configurations to improve classification performance and robustness.

---

## 🎯 Objectives

* Build a classification model for ECG-based arrhythmia detection
* Address class imbalance using SMOTEENN technique
* Improve prediction performance through ensemble learning
* Evaluate model performance using classification metrics

---

## 📊 Dataset

* **Source**: MIT-BIH Arrhythmia Dataset
* **Type**: ECG time-series data
* **Classes**:

  * N (Normal)
  * S (Supraventricular)
  * V (Ventricular)
  * F (Fusion)
  * Q (Unknown)

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Train-test split with stratification
* Normalization of ECG signals
* Handling class imbalance using **SMOTEENN** (combination of oversampling & undersampling)

### 2. Model Architecture

* 1D Convolutional Neural Network (CNN) for feature extraction

* Layers used:

  * Conv1D
  * MaxPooling1D
  * Batch Normalization
  * Dropout
  * Dense layer

* Multiple CNN models trained with different kernel sizes

### 3. Ensemble Learning

* Three CNN models trained independently
* Final prediction obtained using **probability averaging (soft voting)**
* Improves generalization and reduces overfitting

---

## 🚀 Tech Stack

* Python
* TensorFlow / Keras
* Scikit-learn
* Imbalanced-learn (SMOTEENN)
* Pandas, NumPy
* Matplotlib, Seaborn

---

## 📈 Results

* Accuracy: 96,79%
* Precision (weighted): 97,59%
* Recall (Weighted): 96,79%
* F1-Score (Weighted): 97,07%

### 📊 Evaluation

* Classification Report
* Confusion Matrix
* Learning Curve (Accuracy & Loss)

