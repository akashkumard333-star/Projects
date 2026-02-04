# 🫀 Heart Health Alert System  
### End-to-End Machine Learning Pipeline Using AWS EMR, SageMaker, Lambda, SNS, Athena, and S3

---

## 🧭 Project Overview

This project implements a complete cloud-based **heart attack risk prediction and alerting system** using Amazon Web Services.  
It simulates patient vitals, processes health data at scale, trains an **XGBoost model**, generates real-time predictions with **AWS Lambda**, triggers alerts via **Amazon SNS**, and enables analytics using **Amazon Athena**.

The system mirrors how modern hospitals and remote patient-monitoring platforms use **cloud-native machine learning pipelines** for proactive cardiac risk assessment.

---

## 📊 Final Deliverables

### **1. End-to-End AWS ML Pipeline**
A fully operational pipeline integrating:
- **Amazon S3** – Data lake & ingestion  
- **AWS EMR (Spark)** – Distributed preprocessing  
- **Amazon SageMaker** – Model training & deployment  
- **AWS Lambda** – Automated real-time inference  
- **Amazon SNS** – High-risk alerts  
- **Amazon Athena** – Analytics & reporting  

---

### **2. SNS High-Risk Alert**
_Email alert triggered when predicted risk exceeds threshold (0.45)_  
<!-- Add your SNS screenshot here -->
<img width="940" height="529" alt="image" src="https://github.com/akashkumard333-star/akashkumard333/blob/d005f96e9d16946f9af3b0347b02189f60f95a6e/assets/SNS.png" />


---

### **3. Athena Analytics**
_Analytics on high-risk patients, age groups, sleep correlation, and activity patterns_  
<!-- Add Athena screenshots here -->
<img width="940" height="529" alt="image" src="https://github.com/akashkumard333-star/akashkumard333/blob/d005f96e9d16946f9af3b0347b02189f60f95a6e/assets/Athena.png" />

---

### **4. Cluster**
_Distributed Spark cluster used for large-scale vitals aggregation_  
<!-- Add Athena screenshots here -->
<img width="940" height="529" alt="image" src="https://github.com/akashkumard333-star/akashkumard333/blob/d005f96e9d16946f9af3b0347b02189f60f95a6e/assets/Cluster.png" />

---

### **5. EMR**
<img width="940" height="529" alt="image" src="https://github.com/akashkumard333-star/akashkumard333/blob/d005f96e9d16946f9af3b0347b02189f60f95a6e/assets/EMR.png" />

---

### **5. Dataset**
_Simulated and historical datasets used for training and inference_ 
<img width="940" height="529" alt="image" src="https://github.com/akashkumard333-star/akashkumard333/blob/d005f96e9d16946f9af3b0347b02189f60f95a6e/assets/dataset.png" />



---

## 🧩 Project Phases

---

## **Phase I – Data Generation & Ingestion**
- Generated **7-day simulated vitals** for 20 patients
- Simulated realistic heart rate, blood pressure, sleep, and activity data
- Uploaded simulated and historical datasets to **Amazon S3**

**Output:** `simulated_vitals.csv`

**Files:**
```text
phase1/
 ├─ generate_simulated.py
 └─ upload_to_s3.sh
```
---
## **Phase II – Distributed Data Processing (AWS EMR + Spark)**
- Aggregated daily patient vitals into **weekly averages**
- Cleaned and transformed historical heart health data
- Joined simulated and historical datasets using **Patient ID**
- Stored processed dataset back into **Amazon S3**

**Output:** `processed_heart_health_data.csv`

**Files:**
```text
phase2/
 └─ Spark job executed on AWS EMR cluster
```
---
## **Phase III – Machine Learning Model (Amazon SageMaker)**
- Performed feature engineering and preprocessing for ML readiness
- Trained an **XGBoost binary classification model** for heart attack risk prediction
- Evaluated model performance using **AUC**
- Deployed a real-time inference endpoint on **Amazon SageMaker**

**Output:** `processed_heart_health_data.csv`

**Files:**
```text
phase3/
 └─ Model training and deployment configured in SageMaker

```
---
## **Phase IV – Real-Time Prediction & Alerts (AWS Lambda + SNS)**
- Implemented serverless inference using **AWS Lambda**
- Integrated Lambda with the SageMaker inference endpoint
- Generated real-time predictions for incoming patient vitals
- Triggered **Amazon SNS email alerts** for high-risk patients

**Output:** `Real-time prediction results`
            `SNS email notifications`

**Files:**
```text
phase4/
 └─ AWS Lambda function and SNS configuration

```
---
## **Phase V – Analytics & Reporting (Amazon Athena)**
- Created Athena external tables over processed and prediction datasets
- Executed SQL queries for healthcare risk analysis
- Analyzed age-based risk patterns and sleep-duration correlations
- Generated analytical insights for clinical decision support
**Output:** `Athena query results`
            `Analytical insights and reports`
**Files:**
```text
phase5/
 └─ Athena SQL queries and analytics execution

```
---

## 🧠 Dataset Overview

### **Synthetic Patient Vitals (Phase I)**
Simulated data representing **20 patients over a 7-day period**, designed to mimic real-world health monitoring signals.

**Captured attributes include:**
- Heart rate  
- Blood pressure (systolic & diastolic)  
- Sleep duration  
- Physical activity level  
- Timestamp  

---

### **Historical Heart Health Dataset**
Publicly available heart attack prediction dataset sourced from Kaggle:  
https://www.kaggle.com/datasets/iamsouravbanerjee/heart-attack-prediction-dataset

**Key features:**
- Demographics: age, sex  
- Clinical indicators: cholesterol, blood pressure, diabetes  
- Lifestyle metrics: BMI, stress level, exercise hours  
- Target label: heart attack risk  

---

## 👥 Target Users & Stakeholders

- Cardiology and emergency response teams  
- Healthcare data analysts  
- Insurance and risk assessment professionals  
- Clinical researchers and academic institutions  
- Remote patient monitoring platforms  

---

## 💡 Insights & Outcomes

- Identification of patients with elevated cardiac risk  
- Relationship between sleep duration and predicted risk levels  
- Age-based stratification of heart attack likelihood  
- Impact of physical activity on heart rate and model predictions  
