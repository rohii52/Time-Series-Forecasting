# Time Series & Forecasting

## Overview
This repository contains research and analysis on **Time Series & Forecasting**, focusing on two primary case studies:

1. **Average Annual Temperature Analysis in the Midlands (1900-2021)**  
2. **House Price Prediction in the East Midlands (2010-2020)**

The project applies **time series modeling techniques** such as **ARIMA** and **SARIMA** to predict future trends in climate change and the housing market. 

## Datasets
The datasets used in this research include:
- **Temperature Data (1900-2021)**: Average annual temperature of the Midlands region, recorded by the UK Meteorological Office Hadley Climate Centre.
- **House Price Data (2010-2020)**: Monthly average house prices in the East Midlands, extracted from housing market data.

## Research Questions
- **Question 1**: How have temperature patterns evolved in the Midlands over 122 years? Can we forecast future climate trends?
- **Question 2**: What are the historical trends in housing prices in the East Midlands, and can we predict future property values?

---

## Methodology

### **1. Temperature Analysis (1900-2021)**
#### **Exploratory Data Analysis (EDA)**
- Time Series visualization with **trend analysis**
- **LOESS smoothing** to capture fluctuations
- **Augmented Dickey-Fuller (ADF) test** to assess stationarity

#### **Modeling Approach**
- Applied **ARIMA(0,1,1)** after differencing to handle non-stationarity
- Evaluated **ACF & PACF plots** for model selection
- Diagnostic tests: **Ljung-Box test**, **Jarque-Bera test**, **Residual Analysis**
- Forecasted **future temperature trends** for the Midlands

### **2. House Price Forecasting (2010-2020)**
#### **Exploratory Data Analysis (EDA)**
- Seasonal and trend decomposition
- Time series visualization of monthly price variations
- Stationarity check using **ADF test**

#### **Modeling Approach**
- Implemented **SARIMA(1,1,2)(0,1,1)[12]** for seasonal adjustments
- Model evaluation using **AIC, BIC, and error metrics**
- Forecasted **house prices for Jan-June 2020**

---

## Results
- **Temperature Trends**: The ARIMA(0,1,1) model indicates a warming trend in the Midlands, aligned with global climate change patterns.
- **House Price Predictions**: The SARIMA model forecasts **steady growth in property values** in the East Midlands, with increased uncertainty in long-term projections.

---

## Repository Structure
```
├── Dataset
│   ├── cet_temp.csv (Temperature Data)
│   ├── em_house_prices.csv (House Prices Data)
│
├── Paperwork
│   ├── Assignment.pdf (Research Questions & Details)
│   ├── Paperwork.pdf (Full Research Report)
│
├── RMD (Research & Methodology Documents)
│   ├── Question-1.pdf (Temperature Analysis)
│   ├── Question-2.pdf (House Price Forecasting)
│
├── Source Code
│   ├── Q1_code.Rmd (Temperature Modeling)
│   ├── Q2_code.Rmd (House Price Modeling)
│   ├── forecasted_prices.csv (Predicted House Prices)
│   ├── rounded_forecasted_prices.csv (Rounded Predictions)
│
└── README.md (Project Documentation)
```

---

## Installation & Usage
### **1. Clone Repository**
```bash
git clone https://github.com/yourusername/Time-Series-Forecasting.git
cd Time-Series-Forecasting
```

### **2. Load the Data**
- Ensure the CSV datasets are in the **Dataset/** folder before running the scripts.

### **3. Run the Analysis**
#### **Temperature Forecasting (R)**
```r
source('Source Code/Q1_code.Rmd')
```
#### **House Price Forecasting (R)**
```r
source('Source Code/Q2_code.Rmd')
```

---

## Conclusion
This research demonstrates the effectiveness of **Time Series Forecasting models** for predicting climate trends and real estate price movements. Future improvements may include **machine learning approaches**, additional economic indicators, and multi-variable forecasting models.

---

## Author
[Rohith Ganesan](https://github.com/rohi52)

---

## References
1. UK Meteorological Office Hadley Climate Centre
2. House Price Index Data (2010-2020)
3. University of Nottingham - MATH4022 Time Series & Forecasting

For further information, refer to **Paperwork.pdf** in this repository.
