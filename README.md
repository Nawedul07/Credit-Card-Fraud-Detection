# Credit-Card-Fraud-Detection
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The dataset contains anonymized features derived from actual credit card transactions, including both normal and fraudulent cases.
# Credit Card Fraud Detection

This project is focused on detecting fraudulent credit card transactions using **Logistic Regression**. The dataset used contains anonymized features of transactions, and the goal is to accurately classify transactions as **fraudulent** or **legitimate**.

## 📊 Dataset

The dataset contains the following columns:

- **Time**: Seconds elapsed between each transaction and the first transaction in the dataset.
- **V1 to V28**: Principal components obtained with PCA (anonymized due to confidentiality).
- **Amount**: Transaction amount.
- **Class**: Target variable (0 = Legitimate, 1 = Fraudulent).

> Note: The dataset is highly imbalanced — only a small fraction of transactions are fraudulent.

## 🧠 Model

A **Logistic Regression** model is trained to classify transactions. The model is chosen for its simplicity and interpretability, especially suitable as a baseline.

### Steps Followed:

1. **Data Preprocessing**
   - Handling imbalance using undersampling or SMOTE (as per implementation).
   - Scaling `Amount` and `Time` features (if needed).

2. **Model Training**
   - Logistic Regression with appropriate regularization.
   - Train-test split to evaluate performance.

3. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - ROC-AUC Curve

## 📈 Results

The performance is evaluated based on its ability to detect fraud accurately while minimizing false positives. Given the imbalanced dataset, **Recall** and **ROC-AUC** are critical metrics.

## 📁 Files

- `creditcard.csv` – Input dataset.
- `credit_card_fraud_detection.ipynb` – Jupyter Notebook with full implementation.
- `README.md` – This file.

## ⚙️ Requirements

To run this project, install the following packages:

pip install pandas numpy matplotlib seaborn scikit-learn


🚀 How to Run
Clone this repository:

git clone https://github.com/yourusername/credit-card-fraud-detection.git

Navigate to the project folder and open the notebook:

cd credit-card-fraud-detection
jupyter notebook credit_card_fraud_detection.ipynb


📌 Future Improvements
Use of advanced models like Random Forest, XGBoost, or Neural Networks.

Deploying the model with a web interface using Flask or Streamlit.

Real-time fraud detection pipeline.

👤 Author
Nawedul
B.Tech AIML Student
Passionate about ML, Deep Learning, and solving real-world problems.
