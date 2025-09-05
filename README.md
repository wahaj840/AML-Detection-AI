# AML-Detection-AI  
**Enhancing Anti-Money Laundering (AML) Compliance & Detection with AI**  
MSc Artificial Intelligence – Applied Research Project  
Author: **Ali Wahaj (20026654)**  

---

## 📌 Project Overview
This project explores how **Artificial Intelligence (AI)** and **Machine Learning (ML)** can enhance **Anti-Money Laundering (AML)** detection in the banking sector.  
Traditional AML systems are mostly rule-based, which leads to **high false positives, poor adaptability, and scalability challenges**.  

Using the **SAML-D Synthetic Dataset (9.5M transactions, Kaggle)**, this project applies **advanced ML/DL models** and **feature engineering** to improve detection accuracy, interpretability, and cost-effectiveness.

---

## 🎯 Objectives
- Implement **Temporal Convolutional Networks (TCNs)** and **TCNs with Attention** to capture sequential transaction behaviors.  
- Apply **XGBoost** and **Random Forest** as robust baseline models.  
- Handle **class imbalance** using SMOTE and undersampling.  
- Engineer **temporal, behavioral, and risk-based features** for stronger detection.  
- Evaluate models with **precision, recall, ROC-AUC, and economic impact**.  

---

## 🛠️ Methodology
- **Framework:** CRISP-DM (Cross-Industry Standard Process for Data Mining)  
- **Data Preprocessing:** Outlier removal, scaling, one-hot encoding, high-risk flags  
- **Feature Engineering:**  
  - Transaction time clusters (hour, day, weekday, weekend)  
  - Sender-receiver frequency ratios  
  - Rolling 7-day transaction sums & counts  
  - Risk flags (countries, currencies, large amounts)  
- **Models Implemented:**  
  - Random Forest  
  - XGBoost  
  - Temporal Convolutional Network (TCN)  
  - TCN + Attention  

---

## 📊 Key Results
- **TCN (Best Performer):**  
  - Accuracy: **99.61%**  
  - Precision & Recall: **100%**  
  - ROC-AUC: **1.0**  
  - Lowest false positives/negatives → most cost-effective model.  

- **XGBoost:**  
  - Precision: **97%**, Recall: **79%**  
  - Balanced trade-off, cost-efficient alternative.  

- **Random Forest:**  
  - Accuracy: **98.79%** but lower recall → missed laundering cases.  

- **TCN + Attention:**  
  - Perfect recall (100%) but high false positives → increased compliance cost.  

---

## 📂 Repository Contents
- `report/` → Full MSc Applied Research Report (PDF)  
- `presentation/` → Final defense presentation (PPTX)  
- `notebooks/` → Jupyter Notebook with code (EDA, preprocessing, modeling)  
- `dataset/` → (Optional: Sample data or Kaggle link)  
- `requirements.txt` → Python dependencies  

---

## ⚙️ Installation & Usage
```bash
# Clone repository
git clone https://github.com/<your-username>/AML-Detection-AI.git
cd AML-Detection-AI

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook notebooks/Applied_Reseach_Project_Ali_Wahaj_20026654.ipynb
