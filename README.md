# 🏥 Multiple Disease Prediction System

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Status-Live-success?style=for-the-badge)

A machine learning web application that predicts three diseases — Diabetes, Heart Disease, and Parkinson's — based on clinical and biomedical inputs. Built with Python, Scikit-learn, and Streamlit.

🔴 **Live Demo:** [Click Here to Try the App](https://multiple-disease-prediction-balfa6nnnvdxh6xyeao3yz.streamlit.app)

---

## 🎯 Diseases Predicted

| Disease | Algorithm | Dataset Size | Test Accuracy |
|---|---|---|---|
| 🩸 Diabetes | SVM (Linear Kernel) | 768 patients, 8 features | 77.3% |
| ❤️ Heart Disease | Logistic Regression | 303 patients, 13 features | 81.9% |
| 🧠 Parkinson's Disease | SVM (Linear Kernel) | 195 patients, 22 features | 87.2% |

---

## 👨‍💻 My Contribution

This was a group project. My specific contributions:

- Built the complete **Streamlit interface** (`app.py`) — sidebar navigation, input forms, prediction output, and error handling
- Independently trained and evaluated the **ML models** on all three medical datasets
- Integrated three separately trained models into a **unified multi-disease prediction pipeline**
- Deployed the app live on **Streamlit Cloud**

---

## 📊 Model Details

### 🩸 Diabetes — SVM (Linear Kernel)
- **Dataset:** 768 patients (500 non-diabetic, 268 diabetic)
- **Features:** Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, Age
- **Split:** 80/20 stratified train-test split (614 train / 154 test)
- **Training Accuracy:** 78.3% | **Test Accuracy:** 77.3%

### ❤️ Heart Disease — Logistic Regression
- **Dataset:** 303 patients (165 with disease, 138 without)
- **Features:** Age, Sex, Chest Pain Type, Resting BP, Cholesterol, Fasting Blood Sugar, ECG Results, Max Heart Rate, Exercise Angina, ST Depression, Slope, Major Vessels, Thal
- **Split:** 80/20 stratified train-test split (242 train / 61 test)
- **Training Accuracy:** 85.1% | **Test Accuracy:** 81.9%

### 🧠 Parkinson's Disease — SVM (Linear Kernel)
- **Dataset:** 195 patients (147 with Parkinson's, 48 healthy)
- **Features:** 22 biomedical voice measurements (frequency, jitter, shimmer, noise ratios)
- **Split:** 80/20 train-test split (156 train / 39 test)
- **Training Accuracy:** 87.2% | **Test Accuracy:** 87.2%


## 🗂️ Repository Structure

```
├── app.py                        # Streamlit web app (UI + prediction logic)
├── requirements.txt              # Python dependencies
├── runtime.txt                   # Python runtime version
├── saved_models/
│   ├── diabetes_model.sav        # Trained SVM model for diabetes
│   ├── heart_disease_model.sav   # Trained Logistic Regression model
│   └── parkinsons_model.sav      # Trained SVM model for Parkinson's
├── datasets/
│   ├── diabetes.csv              # 768 patient records
│   ├── heart.csv                 # 303 patient records
│   └── parkinsons.csv            # 195 patient records
├── notebooks/
│   ├── Multiple_disease_prediction_system_-_diabetes.ipynb
│   ├── Multiple_disease_prediction_system_-_heart.ipynb
│   └── Multiple_disease_prediction_system_-_Parkinsons.ipynb
└── screenshots/                  # Streamlit app screenshots
```

---

## ⚙️ Run Locally

```bash
# Clone the repository
git clone https://github.com/ParvGT/Multiple-Disease-Prediction.git
cd Multiple-Disease-Prediction

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

---

## 🔮 Future Improvements

- Replace zero values in diabetes dataset (Insulin, Skin Thickness) with class-wise median — likely improves accuracy
- Try ensemble methods like Random Forest or XGBoost for non-linear patterns
- Apply SMOTE to handle class imbalance in Parkinson's dataset (147 vs 48)
- Implement K-Fold cross-validation for more reliable accuracy estimates
- Add hyperparameter tuning via GridSearchCV

---

## 📬 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ParvGR)
