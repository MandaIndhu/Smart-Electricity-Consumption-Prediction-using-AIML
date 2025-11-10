# Week 1 — Data Collection, Understanding & Cleaning
### Project Title: Smart Electricity Consumption Prediction using AI & ML
### Domain: Energy


## ✅ 1. Objective of Week 1
The objective of Week-1 was to:

- Identify the problem related to energy consumption forecasting  
- Select a suitable, real-world dataset  
- Understand the dataset structure  
- Clean and preprocess the dataset  
- Prepare a final cleaned file ready for Machine Learning  


## ✅ 2. Problem Statement
“To analyze and predict hourly electricity consumption across multiple regions using AI/ML techniques to support better demand forecasting, grid stability, and energy planning.”


## ✅ 3. Dataset Source (Kaggle)
The dataset used in this project is obtained from Kaggle:

**Kaggle Dataset Name: Hourly Energy Consumption**  
Dataset URL:  
https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption

Since the dataset contains multiple large CSV files, GitHub does not support uploading them normally.  
Therefore, **GitHub Large File Storage (Git LFS)** was used to upload the dataset.

### ✅ Files Stored Using Git LFS:

Git LFS allows storing dataset files larger than 100 MB in GitHub.

## ✅ 4. Dataset Description
The dataset contains hourly electricity consumption from multiple regions within the PJM Interconnection.

**Main columns:**

- Datetime  
- AEP_MW  
- COMED_MW  
- DAYTON_MW  
- DEOK_MW  
- DOM_MW  
- DUQ_MW  
- EKPC_MW  
- FE_MW  
- NI_MW  
- PJME_MW  
- PJMW_MW  
- PJM_Load  
- PJM_Load_MW  

Total columns: **25**  
Total records: **hundreds of thousands of hourly entries**

## ✅ 5. Data Cleaning Performed
Several steps were applied to prepare the dataset:

### ✅ Step 1: Parsing and Indexing Datetime  
Converted `Datetime` column to datetime type and set it as index.

### ✅ Step 2: Cleaning Missing & Duplicate Values  
- Removed NaN rows  
- Removed repeated timestamps  

### ✅ Step 3: Standardizing Column Names  
Stripped whitespace and ensured consistent format.

### ✅ Step 4: Ensuring Numeric Values  
Converted all *_MW columns to numeric format.

### ✅ Step 5: Saving the Cleaned Data  
Final dataset saved as:

This file is uploaded using **Git LFS**.

## ✅ 6. Week-1 Deliverables
- Problem Statement  
- Dataset Source  
- Data Understanding  
- Data Cleaning  
- Final Cleaned File  
- Uploaded Dataset using Git LFS  

## ✅ 7. Conclusion (Week 1)
Week-1 successfully prepared the dataset for ML.  
The cleaned dataset is reliable, structured, and production-ready for Week-2 and Week-3 models.

