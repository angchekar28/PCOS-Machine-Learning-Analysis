# 🔍 PCOS Diagnosis: Machine Learning Model Comparison  

## 📌 Overview  
This project evaluates various **machine learning models** for diagnosing **Polycystic Ovary Syndrome (PCOS)** based on medical and clinical features. The goal is to determine the most **accurate and efficient** model for predicting PCOS while analyzing execution time and classification metrics.  

## 📊 Dataset  
The dataset contains medical records of individuals, including various physiological and lifestyle-related parameters that may influence PCOS diagnosis.  

### Features:  
- **Independent Variables:** Age, BMI, Insulin levels, LH/FSH ratio, Follicle count, etc.  
- **Target Variable:** Presence or absence of PCOS (Binary: 1 = PCOS, 0 = No PCOS)  

## 🛠️ Technologies Used  
- **Python** (pandas, numpy, scikit-learn, XGBoost)  
- **Jupyter Notebook/Kaggle/Colab**  
- **Matplotlib & Seaborn** for visualization  

## 🚀 Models Implemented  
The following classification models were evaluated:  

1. **Random Forest**  
2. **Logistic Regression**  
3. **Support Vector Machine (RBF & Linear)**  
4. **K-Nearest Neighbors**  
5. **Decision Tree**  
6. **XGBoost**  
7. **Naive Bayes**  

## 📈 Model Performance Comparison  

| Model                         | Accuracy | Precision (Class 1) | Recall (Class 1) | F1-Score (Class 1) | Implementation Time (s) |
|-------------------------------|----------|---------------------|------------------|-------------------|--------------------------|
| Random Forest                 | 99.00%   | 0.99                | 0.95             | 0.97              | 0.1783                   |
| Logistic Regression           | 88.50%   | 0.72                | 0.67             | 0.69              | 0.0059                   |
| SVM (RBF Kernel)              | 96.00%   | 0.90                | 0.90             | 0.90              | 0.0089                   |
| SVM (Linear Kernel)           | 89.50%   | 0.74                | 0.72             | 0.73              | 0.0100                   |
| K-Nearest Neighbors           | 96.50%   | 0.92                | 0.90             | 0.91              | 0.0132                   |
| Decision Tree                 | 99.50%   | 1.00                | 0.97             | 0.99              | 0.0026                   |
| XGBoost                       | 99.50%   | 1.00                | 0.97             | 0.99              | 0.0332                   |
| Naive Bayes                   | 69.50%   | 0.39                | 1.00             | 0.56              | 0.0019                   |

## 🏆 Conclusion  

### ✅ Best Model Choices:  
1. **Decision Tree & XGBoost** – Highest accuracy (99.50%) with strong precision, recall, and F1-scores. Decision Tree was the fastest among them (0.0026s).  
2. **Random Forest** – Excellent accuracy (99%) but had the longest execution time (0.1783s).  
3. **SVM (RBF) & KNN** – Reliable models with **96%+ accuracy**, but KNN took slightly more time (0.0132s).  

### ⚡ Performance vs. Speed:  
- **Fastest Model:** Naive Bayes (0.0019s), but it had the lowest accuracy (69.50%).  
- **Balanced Performance:** XGBoost and Decision Tree provide the best trade-off between accuracy and execution time.  

### ❌ Weak Model Choices:  
- **Naive Bayes** struggled significantly due to **class imbalance**, making it unsuitable.  
- **Logistic Regression & Linear SVM** had moderate performance but **struggled with Class 1 predictions**.  

### 🔥 Final Recommendation:  
For **high accuracy and efficiency**, **Decision Tree or XGBoost** are the best choices. If **speed is not a constraint**, **Random Forest** is also an excellent option.  

## 🔧 Installation & Usage  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/yourusername/PCOS-ML-Model-Comparison.git
cd PCOS-ML-Model-Comparison
```
### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
### 3️⃣ Run the Jupyter Notebook
```bash
jupyter notebook

