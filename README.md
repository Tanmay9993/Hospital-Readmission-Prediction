# 🏥 Hospital Readmission Risk Prediction

## 🔍 Overview
This project uses machine learning to predict 28-day hospital readmissions among heart failure patients using clinical, demographic, and comorbidity data. It combines feature importance analysis with robust modeling and resampling techniques to identify high-risk cases.

## 🎯 Purpose & Problem Statement
Preventable readmissions are costly for hospitals and risky for patients. Under the HRRP policy, hospitals face Medicare penalties for excessive 30-day readmission rates. This project helps healthcare providers identify patients at risk of early readmission and take preventive action through better planning and monitoring.

## 🛠️ Key Features & Workflow
- **Data Volume**: 2,000+ heart failure patient records, 15,000+ medication records
- **Tools Used**: Python, Pandas, Scikit-learn, XGBoost, LightGBM, SHAP, SMOTE
- **Analytics & ML Tasks**:
  - Visualized readmission patterns across visits, conditions, and vitals
  - Used SHAP and Random Forest to rank important features (e.g., chloride, comorbidities, medication count)
  - Trained and compared models (Logistic Regression, SVM, RF, XGBoost, LightGBM)
  - Addressed class imbalance with SMOTE to boost recall of readmitted patients
- **Best Result**: Post-SMOTE LightGBM achieved ~91% accuracy with improved recall

## 📈 Results & Visuals

### 🔹 SHAP Summary Plot
Explains global impact of comorbidities on readmission risk.
![download (2)](https://github.com/user-attachments/assets/3709fa43-4720-4ef6-b8f6-f09de46aa416)


### 🔹 Readmission Rate by NYHA Class
![download (1)](https://github.com/user-attachments/assets/fe76a500-19a2-4c57-a44f-89ef1488b357)

### 🔹 Readmission Rate by Medication Count
![download (5)](https://github.com/user-attachments/assets/4df212e7-7f8e-4e07-ac4f-1f643dc67513)

### 🔹 Readmission Rate by Weight
![download (7)](https://github.com/user-attachments/assets/c8b2b278-8a93-4612-af3f-805525522287)

---

## <h1>Data Source</h1> 
This project uses the [Hospitalized patients with heart failure: integrating electronic healthcare records and external outcome data](https://physionet.org/content/heart-failure-zigong/1.3/).  

<h3>Database:</h3>
Zhang, Z., Cao, L., Zhao, Y., Xu, Z., Chen, R., Lv, L., and Xu, P. (2022) 'Hospitalized patients with heart failure: integrating electronic healthcare records and external outcome data' 
(version 1.3), PhysioNet. Available at: https://doi.org/10.13026/5m60-vs44.
<br></br>
Zhang, Z., Cao, L., Chen, R. et al. Electronic healthcare records and external outcome data for hospitalized patients with heart failure. 
Sci Data 8, 46 (2021). https://doi.org/10.1038/s41597-021-00835-9

<h3>Physionet</h3>
Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P.C., Mark, R., Mietus, J.E., Moody, G.B., Peng, C.K. and Stanley, H.E., 
2000. PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. Circulation [Online]. 
101 (23), pp. e215–e220.
