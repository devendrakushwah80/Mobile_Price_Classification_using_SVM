# 📱 Mobile Price Classification using SVM

## 📌 Project Overview

This project focuses on classifying mobile phones into different price ranges based on their technical specifications using a Support Vector Machine (SVM).

The notebook follows a structured machine learning pipeline including data analysis, preprocessing, model training, and evaluation, with special emphasis on kernel-based learning.

---

## 🧠 Problem Statement

Given various mobile phone features such as battery power, RAM, internal memory, camera specifications, and connectivity options, the objective is to predict the price range (`price_range`) of a mobile phone.

The target variable is multi-class, representing increasing levels of mobile phone prices.

---

## 📂 Dataset Description

- **File:** `train.csv`
- **Target Variable:** `price_range`
- **Features:** All numerical mobile specifications
- **Missing Values:** None
- **Duplicate Rows:** None

The dataset is clean and suitable for classical machine learning algorithms.

---

## 🔍 Exploratory Data Analysis (EDA)

The following EDA steps were performed:

- Dataset shape and data types inspection
- Statistical summary using `describe()`
- Correlation analysis
- Correlation heatmap visualization
- Feature distribution analysis
- Unique value analysis per feature

Key observations from EDA helped in understanding feature relationships with the target variable.

---

## ⚙️ Data Preprocessing

### Feature and Target Separation
- `X`: Feature matrix
- `y`: Target variable (`price_range`)

### Train-Test Split
- Training data: 80%
- Testing data: 20%
- `random_state = 42`

### Feature Scaling
- StandardScaler used for normalization
- Implemented using ColumnTransformer
- Essential for distance-based models like SVM

---

## 🤖 Model Used

### Support Vector Machine (SVM)

Initial configuration:
- Kernel: RBF
- C: 1.0
- Gamma: scale

SVM is chosen due to its effectiveness in high-dimensional spaces and ability to model non-linear decision boundaries.

---

## 📈 Model Evaluation

Model performance was evaluated using:

- Accuracy Score
- Classification Report (Precision, Recall, F1-score)
- Confusion Matrix

These metrics provide both overall and class-wise performance insights.

---

## 🔬 Kernel Comparison

Different SVM kernels were evaluated to analyze their impact on model performance:

- Linear Kernel
- RBF Kernel
- Polynomial Kernel

Accuracy scores were compared across kernels to understand kernel sensitivity.

---

## 🧪 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📁 Project Structure

├── Mobile_Price_Classifier.ipynb
├── train.csv
├── README.md
└── requirements.txt


---

## 🚀 Key Learnings

- Importance of feature scaling for SVM
- Impact of kernel choice on classification performance
- Role of EDA in understanding data behavior
- Need for detailed evaluation beyond accuracy

---

## 🎯 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Cross-validation for better generalization
- Comparison with other classification algorithms
- Feature importance analysis using model-agnostic methods

---

## 📌 Conclusion

This project demonstrates a structured machine learning workflow using Support Vector Machines for multi-class classification. It emphasizes strong fundamentals, proper preprocessing, and thoughtful model evaluation rather than relying on black-box predictions.
