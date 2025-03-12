# Weather Trend Forecasting - PM Accelerator Assessment  

## Project Overview  
This project is part of the **PM Accelerator** program and focuses on analyzing and forecasting global weather trends using machine learning and data science techniques. The dataset used is the **Global Weather Repository**, which contains over 40 weather-related features from locations worldwide. The project involves data preprocessing, exploratory data analysis (EDA), time-series forecasting, anomaly detection, feature importance analysis, and spatial analysis.  

## PM Accelerator Mission  
The PM Accelerator program is designed to enhance data science expertise by applying real-world datasets to solve complex problems. This assessment evaluates skills in data cleaning, visualization, forecasting, and climate pattern analysis.  

## Dataset Information  
- **Dataset Name**: [Global Weather Repository](https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository/code)  
- **Size**: 40+ features, Daily weather data for cities worldwide  
- **Source**: Kaggle  
- **Key Features**:  
  - Temperature, Humidity, Wind Speed, Pressure, Precipitation  
  - Air Quality (PM2.5, PM10, NO2, Ozone)  
  - Geographic Information (Latitude, Longitude, Country)  

---

## Methodology  

### Data Preprocessing  
- Handled missing values (numerical: median, categorical: mode).  
- Removed outliers using **Z-score filtering**.  
- Normalized numerical features using **MinMaxScaler**.  
- Converted timestamps for **time-series forecasting**.  
- Dropped unnecessary columns for model efficiency.  

### Exploratory Data Analysis (EDA)  
- **Correlation Heatmap** – Shows relationships between weather variables.  
- **Temperature Trends Over Time** – Analyzed trends in various locations.  
- **Precipitation Distribution by Country** – Explored rainfall patterns.  
- **Boxplots for Outlier Detection** – Identified extreme weather conditions.  

### Forecasting Models  
The following models were implemented to forecast temperature trends:  

| Model       | Type | Strengths |
|-------------|-------------|-------------|
| **ARIMA** | Time Series | Best for linear trends and short-term forecasts |
| **Prophet** | Time Series | Captures seasonality and external regressors |
| **Random Forest** | Machine Learning | Handles non-linear relationships well |
| **XGBoost** | Machine Learning | High accuracy and fast computation |

#### Model Performance Evaluation  
- Metrics used: **Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score**.  
- Models were compared to identify the best-performing technique.  

### Advanced Analysis  
- **Anomaly Detection** – Using **Isolation Forest** to identify unusual weather patterns.  
- **Feature Importance** – Random Forest and XGBoost were used to rank key weather predictors.  
- **Environmental Impact Study** – Analyzed the correlation between air quality and weather conditions.  
- **Geospatial Analysis** – Mapped temperature distributions across countries.  

---

## Key Insights  
- **XGBoost and Prophet** provided the most accurate forecasts.  
- **Seasonal variations significantly impact temperature and precipitation trends**.  
- **Poor air quality is linked to rising temperatures in urban areas**.  
- **Anomaly detection identified extreme climate fluctuations**.  

## How to Run the Project  

### Prerequisites  
Ensure you have the required libraries installed:  
```bash
pip install pandas numpy seaborn matplotlib sklearn statsmodels geopandas prophet xgboost
