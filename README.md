# Diabetes Risk Prediction: Biomarkers vs. Lifestyle Factors

🔍 **Can we predict diabetes risk without blood tests?**  
This project compares machine learning models trained on **clinical biomarkers** (HbA1c, blood glucose) versus **lifestyle/demographic factors** (age, BMI, smoking history) to assess their effectiveness in diabetes risk prediction.

## 📌 Key Objectives
- **Predict diabetes risk** using non-invasive, easily accessible features (no blood tests).  
- **Identify key predictors** (e.g., BMI, hypertension) through feature importance analysis.  
- **Benchmark performance** against clinical baselines (HbA1c > 6.5%) and state-of-the-art models.  

## 📂 Dataset  
- **Source**: [Diabetes Prediction Dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset) (20,000 samples).  
- **Features**:  
  - *Excluded*: HbA1c, Blood Glucose (for non-blood models).  
  - *Included*: Age, Gender, BMI, Hypertension, Heart Disease, Smoking History.  

## 🤖 Models & Approach  
1. **Baseline Models**:  
   - **Clinical Rule**: Diagnose diabetes if HbA1c > 6.5%.  
   - **Logistic Regression**: Trained on HbA1c and blood glucose.  
2. **Lifestyle/Demographic Models**:  
   - **XGBoost**, **Random Forest**, **Logistic Regression** (trained without blood tests).  
3. **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, AUC-ROC.  

## 🚀 Results  
| Model Type          | Accuracy | AUC-ROC | Key Findings                          |  
|---------------------|----------|---------|---------------------------------------|  
| Clinical Rule       | XX%      | -       | Relies solely on HbA1c threshold.     |  
| Blood Test (Logistic)| XX%      | XX%     | Simple but requires lab data.         |  
| **Lifestyle (XGBoost)** | **XX%** | **XX%** | Achieved comparable performance without blood tests. |  

- **Top Predictors**: BMI, Age, Hypertension (identified via SHAP values).  

## 🛠️ Tools  
- **Python Libraries**: Pandas, Scikit-learn, XGBoost, SHAP, Matplotlib/Seaborn.  
- **Techniques**: Feature engineering, hyperparameter tuning, cross-validation.  

## 🌍 Impact  
This work demonstrates the potential of **non-invasive diabetes screening** using lifestyle and demographic data, offering a low-cost alternative for early detection in resource-limited settings.  

📊 **Repo Structure**:  
data/
models/
notebooks/
results/
README.md
---

💡 **Why This Matters**:  
Early diabetes prediction without blood tests could revolutionize preventive healthcare, especially in regions lacking lab infrastructure.  