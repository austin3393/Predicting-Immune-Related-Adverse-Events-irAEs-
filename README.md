# 🧬 Predicting Immune-Related Adverse Events (irAEs) in ICI Therapy  

## 📌 Overview  
This project develops a machine learning framework to predict **immune-related adverse events (irAEs)** in melanoma patients treated with **immune checkpoint inhibitors (ICIs)**.  
The work was conducted in collaboration with the **Lombardi Comprehensive Cancer Center (LCCC)** as part of a graduate capstone project in Health Informatics & Data Science.  

Immune checkpoint inhibitors (PD-1, PD-L1, CTLA-4) have revolutionized oncology care but carry high risk of irAEs — unpredictable, potentially severe inflammatory reactions that may lead to hospitalization, permanent organ dysfunction, or early discontinuation of therapy. Current clinical guidelines emphasize **reactive management** of irAEs, but proactive **risk stratification** tools are lacking.  

This project explores whether **EHR-derived clinical and demographic data** can support **pre-treatment prediction of irAEs**, offering potential to guide monitoring, decision-making, and personalized care.  

---

## 🎯 Goals  
- Build and evaluate ML models to predict occurrence of irAEs.  
- Explore predictive power of **clinical, demographic, and comorbidity features**.  
- Provide exploratory data visualizations to uncover patterns in patient cohorts.  
- Establish a baseline modeling pipeline for future integration with genomics, labs, and unstructured notes.  

---

## ⚙️ Methods  
### Data  
- **Source:** Melanoma cohort from LCCC I/O Registry  
- **Features:**  
  - Demographics (age, sex, race)  
  - Clinical comorbidities (Charlson Comorbidity Index, autoimmune history)  
  - Cancer/treatment variables (ICI regimen, cancer type, line of therapy)  
  - Outcomes: Occurrence of irAE (binary classification)  

### Approach  
1. **Data Preprocessing:**  
   - Feature selection & harmonization  
   - Handling missingness (dropping high-missing variables, removing incomplete records)  
   - Low-variance feature pruning  
2. **Exploratory Data Analysis:**  
   - Cohort breakdown by demographics, comorbidities, and ICI regimens  
   - irAE prevalence visualization across subgroups  
3. **Modeling:**  
   - Baseline classifiers (Logistic Regression, Random Forest, XGBoost)  
   - AUROC evaluation of predictive features  
   - Comparison of model performance vs. univariate predictors  

---

## 📊 Key Findings  
- **irAEs were common** across the cohort, with variability by treatment regimen.  
- Certain comorbidities and demographics showed **signal in feature importance analysis**, though predictive power was modest.  
- Baseline models achieved **AUROC ~0.65**, establishing proof-of-concept for structured EHR-based prediction.  
- Missingness and cohort size remain major barriers, underscoring the need for **multi-institutional datasets** and **integration of labs/genomics**.  

---

## 🛠️ Tools & Technologies  
- **Languages:** Python, SQL  
- **Libraries:** scikit-learn, pandas, matplotlib, seaborn  
- **Data Handling:** REDCap export, feature engineering, cohort preprocessing  
- **Visualization:** matplotlib, seaborn  

---

## 🚀 Future Directions  
- Incorporate **time-series labs** (e.g., blood counts, liver enzymes).  
- Extract **adverse event mentions** from **unstructured notes** via NLP.  
- Expand dataset with **multi-site harmonization** to improve model generalizability.  
- Explore **survival analysis & competing risk models** for time-to-event irAEs.  

---

## 👥 Contributors  
- **Austin Cherian** — Health Informatics & Data Science Graduate Student  
- **Advisors:** Yili Zhang, PhD; Adil Alaoui, PhD; Neil Shah, MD (LCCC)  

---

## 📬 Connect  
- LinkedIn: [linkedin.com/in/austin-cherian](https://linkedin.com/in/austin-cherian)  
- GitHub: [github.com/austin3393](https://github.com/austin3393)  
