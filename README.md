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
https://github.com/preetikumar20/Capstone_Covid19/blob/a871861f8f05c0c51227f05e58bcdd50e33ce2d5/final_capstone_preetidubey.ipynb

## Visualization 
![image](https://github.com/user-attachments/assets/2f58231f-a5cb-4fd4-a280-ade3b31cfa8d)
![newplot](https://github.com/user-attachments/assets/bb35cdad-b468-43af-af75-89a5507725b1)

![percentage_deaths_country](https://github.com/user-attachments/assets/f6c3822b-7d09-4a7c-9b82-8a7db147bc91)

![image](https://github.com/user-attachments/assets/2c961f79-5d3e-41c0-a9f5-ad2976b14c60)


![exog_sarima_fit](https://github.com/user-attachments/assets/5f3bc53b-ef67-41f0-b6ae-d335eda49003)

![image](https://github.com/user-attachments/assets/9e49ff99-375e-4277-8949-0b8356310035)

![Screenshot 2025-03-19 at 1 31 46 AM](https://github.com/user-attachments/assets/3a506882-7dec-4896-8e36-a6ac5108a016)


## Contributors
- **Preeti Dubey**
- Email: preetiup28@gmail.com


