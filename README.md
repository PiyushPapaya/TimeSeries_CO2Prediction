# TimeSeries_CO2Prediction

This project is an introductory time-series forecasting analysis on atmospheric CO₂ data. It combines linear regression, lag features, a deterministic process for trend modeling, and Fourier terms for capturing seasonality. The goal is to model the trend, seasonal patterns, and temporal dependencies in the data and generate forecasts.

The dataset used is the [CO₂ concentration dataset](https://www.statsmodels.org/dev/datasets/generated/co2.html).

---

## About the Dataset

The dataset contains atmospheric CO₂ measurements from continuous air samples collected at the Mauna Loa Observatory, Hawaii, U.S.A.

- **Period of record:** March 1958 - December 2001  
- **Number of observations:** 2,225  
- **Number of variables:** 2  

**Variable definitions:**

- `date` - Sample date  
- `co2` - CO₂ concentration in ppmv  

**First few rows:**

| date       | co2   |
|------------|-------|
| 1958-03-29 | 316.1 |
| 1958-04-05 | 317.3 |
| 1958-04-12 | 317.6 |
| 1958-04-19 | 317.5 |
| 1958-04-26 | 316.4 |

**Summary statistics:**

|      | co2       |
|------|-----------|
| count| 2225.0    |
| mean | 340.14    |
| std  | 17.00     |
| min  | 313.0     |
| 25%  | 324.8     |
| 50%  | 338.3     |
| 75%  | 354.8     |
| max  | 373.9     |

---

## About the Notebook

The notebook walks through the process of modeling and forecasting CO₂ using time-series techniques. It contains the following sections:

- **Import Libraries**
- **Load CO₂ Dataset**
- **Basic Plot of CO₂ Levels**
- **Linear Trend Model**
  - Add a time index  
  - Fit a linear regression model  
  - Plot predictions vs actual data  
- **Lag Feature Model**
  - Create lagged features  
  - Train regression  
  - Visualize predictions  
- **Moving Average Trend**
  - Smooth the data to identify long-term trends  
- **Polynomial Trend with DeterministicProcess**
  - Build a polynomial trend matrix  
  - Fit the trend model  
  - Visualize trend fit  
- **Forecasting Future Values**
  - Generate future design matrix  
  - Predict future CO₂ values  
  - Plot trend forecast  
- **Seasonal Model (Fourier + Trend)**
  - Prepare weekly data  
  - Build Fourier seasonal matrix  
  - Fit model and forecast future values  
  - Plot seasonal fit and forecast  

---

Notebook created and trained on [Kaggle](https://www.kaggle.com) by **Piyush Nagpal**.  
Published on **16 November 2025**.
