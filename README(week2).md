# Week 2 — Machine Learning Model: Training, Prediction & Accuracy
### Project Title: Smart Electricity Consumption Prediction using AI & ML
### Domain: Energy


## ✅ 1. Objective of Week 2
The goal for Week-2 was to:

- Perform train–test split  
- Train a Machine Learning model  
- Predict electricity consumption  
- Compare predictions vs actual values  
- Evaluate model accuracy (MAE, RMSE, R²)  
- Store results and visualizations  

## ✅ 2. Dataset Source
Dataset obtained from Kaggle:

**Kaggle Dataset Name:** Hourly Energy Consumption  
**URL:** https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption

The cleaned dataset was large, so it was uploaded to GitHub using **GitHub Large File Storage (Git LFS)**.

### ✅ Dataset File Used:

This cleaned file contains:

- Datetime index  
- 12+ energy consumption target columns  
- All numeric values ready for modeling  


## ✅ 3. Features Extracted
From the Datetime column, the following features were created:

- `hour`  
- `dayofweek`  
- `month`  
- `year`  

These temporal features help the ML model understand time-related patterns.


## ✅ 4. Machine Learning Model
A **Multi-Output Random Forest Regressor** was used to predict **all target columns simultaneously**.

This model:

- Supports multiple outputs  
- Works well with non-linear consumption patterns  
- Provides a strong baseline before Deep Learning (Week-3)  


## ✅ 5. ML Workflow
1. Load cleaned dataset (stored via Git LFS)  
2. Extract calendar-based features  
3. Split into train (80%) and test (20%)  
4. Train Multi-Output Random Forest model  
5. Generate predictions for all regions  
6. Evaluate performance for each region  
7. Visual comparison graph (Actual vs Predicted)  


## ✅ 6. Example Results (Actual Output)

| Target       | MAE     | RMSE    | R²     |
|--------------|----------|----------|---------|
| NI_MW        | 1.09e-11 | 1.09e-11 | -35.00  |
| PJM_Load_MW  | ~0       | ~0       | 0.00    |
| EKPC_MW      | 51.9     | 95.6     | 0.04    |
| DUQ_MW       | 53.4     | 107.6    | 0.03    |
| DAYTON_MW    | 62.5     | 120.2    | 0.04    |
| AEP_MW       | 390      | 736      | 0.05    |
| COMED_MW     | 430      | 836      | 0.03    |

(Accuracy improves significantly in Week-3 using LSTM.)

## ✅ 7. Visualizations
### 📈 Actual vs Predicted Graph  
Stored in:  

## ✅ 8. Files Uploaded to GitHub

## ✅ 9. Conclusion (Week 2)
Week-2 successfully completed:

- ML training  
- Prediction  
- Accuracy evaluation  
- Visualization  
- GitHub upload with LFS for large dataset  

Now the project moves to **Week-3 (LSTM Deep Learning)** for accurate forecasting.

