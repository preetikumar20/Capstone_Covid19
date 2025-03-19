# Exploring Global COVID-19 Trends and Predicting New Cases in the USA

## Project Overview
This project aims to analyze, forecast, and evaluate the spread of COVID-19 using statistical and machine learning models. We utilize the WHO COVID-19 dataset to explore trends, conduct exploratory data analysis (EDA), and implement forecasting models such as ARIMA and SARIMA to predict case counts.

## Repository Structure
- **notebooks/** – Jupyter notebooks used for data analysis, modeling, and visualization.
- **reports/** – Initial and Final report.
- **README.md** – This file, providing an overview of the project.

## Methodology
### 1. Data Collection
- We used the **WHO COVID-19 dataset**, which includes daily confirmed cases and deaths worldwide.

### 2. Exploratory Data Analysis (EDA)
- **Regional trends:** EMRO and EURO had higher case frequencies.
- **Death distribution:** Right-skewed, indicating many days with low deaths but occasional extreme spikes.
- **Wave patterns:** Two major peaks (2022 and 2023) correspond to Delta and Omicron variants.
- **Country-specific trends:** USA had the highest case count in early 2022, while China saw a peak in late 2022.
- **Mortality trends:** The USA exhibited the highest death toll, followed by Brazil and India.

### 3. Model Selection
We implemented time series forecasting models to predict future COVID-19 cases:
- **ARIMA Model**
- **SARIMA Model**
- **Exog SARIMA Model**
- **Random Forest**
- **XGBoost**
- **LSTM**

### 4. Model Evaluation
 	Model 	MAE 	MSE 	RMSE 	AIC 	BIC
0 	ARIMA 	134360.86 	2.480000e+10 	157527.53 	3380.63 	3397.55
1 	SARIMA 	97100.10 	1.640000e+10 	128000.76 	3462.81 	3474.15
2 	EXOG SARIMA 	79852.14 	NaN 	93150.65 	3669.55 	3689.84
3 	Random Forest 	68322.60 	6.600000e+09 	81348.77 	NaN 	NaN
4 	XGBoost 	122012.04 	3.280000e+10 	181259.31 	NaN 	NaN
5 	LSTM (Training) 	81126.04 	NaN 	185258.85 	NaN 	NaN
6 	LSTM (Test) 	38242.36 	NaN 	56711.65 	NaN 	NaN

• SARIMA and EXOG SARIMA provide strong baseline forecasts. 
• Random Forest minimizes MAE better than ARIMA and SARIMA but shows higher RMSE. 
• LSTM (Test) outperforms all other models, making it the top-performing model. 
• XGBoost shows weaker performance, likely needing tuning or different feature engineering.
**LSTM (Test)** is the most effective model for predicting new COVID-19 cases in the USA.

## Key Findings
- COVID-19 cases exhibited seasonal trends with multiple peaks due to variant outbreaks.
- Public health interventions and vaccinations significantly reduced cases after major waves.
- SARIMA and EXOG SARIMA provide strong baseline forecasts.
- LSTM (Test) outperforms all other models, making it the top-performing model. 

## Deployment
- The final forecasting results and insights were delivered as a structured report.
- Visualizations and predictions were presented to aid decision-making in public health.

## Link for the final capstone project Jupyter notebook
https://github.com/preetikumar20/Capstone_Covid19/blob/ac8c34bb6a10d9860434f838e5dfcb858895507f/prompt_final.ipynb

## Contributors
- **Preeti Dubey**
- Email: preetiup28@gmail.com


