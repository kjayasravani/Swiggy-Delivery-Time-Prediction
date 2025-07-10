# Swiggy Delivery Time Prediction

This project aims to predict the **delivery time of Swiggy food orders** using machine learning models based on rider details, weather, traffic conditions, and geolocation data.

---

## Problem Statement
Predict the food order delivery time based on real-world factors like rider attributes, vehicle type, weather, and traffic. This enables:
- Optimizing delivery operations
- Improving customer satisfaction
- Efficient resource allocation

---

## Business Use Case
- **Customer Satisfaction:** Deliver accurate ETAs and improve transparency.
- **Operational Efficiency:** Better resource and route management for riders.
- **Financial Impact:** Reduce compensation for delays, optimize fuel costs, and boost customer retention.

---

## Dataset
The dataset (`swiggy.csv`) contains:
- Rider details (age, ratings)
- Weather conditions
- Traffic density
- Delivery distance (calculated using geolocation)
- Delivery time in minutes

---

## ML Workflow

### 1. Data Preprocessing
- Handle missing values and outliers
- Feature engineering (delivery distance, time-based features)
- Encoding categorical variables

### 2. Model Building
Models used:
- **Linear Regression** (baseline)
- **Random Forest Regressor** (best performance)

### 3. Model Evaluation
Metrics evaluated:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### 4. Best Model
The **Random Forest Regressor** achieved the best results:
- Lower MAE
- Higher R² on both training and test data

---

## Results
| Model                 | Train MAE | Test MAE | Train R² | Test R² |
|----------------------|-----------|----------|----------|---------|
| Linear Regression     | 12.48     | 13.02    | 0.76     | 0.73    |
| Random Forest         | 9.17      | 10.36    | 0.85     | 0.81    |

---

## Future Improvements
- Use XGBoost or Gradient Boosting models
- Add real-time traffic and weather APIs
- Deploy as a real-time prediction service

---

## Project Structure
```
├── swiggy.csv
├── Data Cleaning.ipynb
├── Food_Delivery_EDA.ipynb
├── data_clean_utils.py
├── swiggy_cleaned.csv
└── model_building.ipynb
```
