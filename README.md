# Exploring Global COVID-19 Trends and Predicting New Cases in the USA

## Project Overview
This project aims to analyze, forecast, and evaluate the spread of COVID-19 using statistical and machine learning models. We utilize the WHO COVID-19 dataset to explore trends, conduct exploratory data analysis (EDA), and implement forecasting models such as ARIMA, SARIMA, Exog SARIMA, Random Forest, XGBoost and LSTM, to predict case counts.

## Repository Structure
- **notebooks/** – Jupyter notebooks used for data analysis, modeling, and visualization.
- **slides/** - PPT file containing highlights of the project.
- **reports/** – Initial and Final report.
- **README.md** – This file, providing an overview of the project.

## Methodology
### 1. Data Collection
- We used the **WHO COVID-19 dataset**, which includes daily confirmed cases and deaths worldwide.

### 2. Exploratory Data Analysis (EDA)
- **Regional trends:** EMRO and EURO had higher case frequencies.
  <img width="864" alt="image" src="https://github.com/user-attachments/assets/75bbf961-1231-494b-858f-176c03c7ed66" />

- **Death distribution:** Right-skewed, indicating many days with low deaths but occasional extreme spikes.
  ![deaths_dist_region](https://github.com/user-attachments/assets/bf1578fe-8bd7-419e-a305-79a0e2f5af4c)

- **Wave patterns:** Two major peaks (2022 and 2023) correspond to Delta and Omicron variants.
  ![cases_over_time_global](https://github.com/user-attachments/assets/c5d0fb12-3f84-46bf-9cb7-dc57e1a3bd96)

- **Country-specific trends:** USA had the highest case count in early 2022, while China saw a peak in late 2022.
  ![percentage_deaths_country](https://github.com/user-attachments/assets/52d7f59c-bcc2-47d4-9be0-51b5b42152e6)

- **Mortality trends:** The USA exhibited the highest death toll, followed by Brazil and India.
  ![deaths_percentage_country](https://github.com/user-attachments/assets/47a77231-4fca-4a09-8aef-253d4f8341d5)


### 3. Model Selection
We implemented time series forecasting models to predict future COVID-19 cases:
- **ARIMA Model**
- **SARIMA Model**
- **Exog SARIMA Model**
- **Random Forest**
- **XGBoost**
- **LSTM**

### 4. Model Evaluation
- MAE,	MSE, 	RMSE used as metrics to determine the best model
  This chart shows the metrics for each model
  ![Screenshot 2025-03-19 at 1 31 46 AM](https://github.com/user-attachments/assets/3a506882-7dec-4896-8e36-a6ac5108a016)

## Key Findings
**EDA**
- The EMRO and EURO regions show a higher frequency of case counts.
- Multiple COVID-19 waves, such as the Delta and Omicron variants.
- The USA recorded the highest number of new cases at the start of 2022, and China had the highest cases by the end of the year.
- The highest death toll was observed in the US, particularly during early 2021 and early 2022, whereas India experienced a massive surge in mid-2021 due to the Delta variant.
**Modeling**
- SARIMA and EXOG SARIMA provide strong baseline forecasts.
  ![exog_sarima_fit](https://github.com/user-attachments/assets/5f3bc53b-ef67-41f0-b6ae-d335eda49003)
  
- Random Forest minimizes MAE better than ARIMA and SARIMA but shows higher RMSE.
- LSTM (Test) outperforms all other models, making it the top-performing model.
- XGBoost shows weaker performance, likely needing tuning or different feature engineering.
- **LSTM (Test)** is the most effective model for predicting new COVID-19 cases in the USA.
  
  ![image](https://github.com/user-attachments/assets/9e49ff99-375e-4277-8949-0b8356310035)


## Deployment
- The final forecasting results and insights were delivered as a structured report.
- Visualizations and predictions were presented to aid decision-making in public health.

## Link for the final capstone project Jupyter notebook
https://github.com/preetikumar20/Capstone_Covid19/blob/a871861f8f05c0c51227f05e58bcdd50e33ce2d5/final_capstone_preetidubey.ipynb

## Visualization 
The distribution of COVID-19 cases on world map
![image](https://github.com/user-attachments/assets/2f58231f-a5cb-4fd4-a280-ade3b31cfa8d)

The distribution of COVID-19 deaths on world map

![newplot](https://github.com/user-attachments/assets/bb35cdad-b468-43af-af75-89a5507725b1)








## Contributors
- **Preeti Dubey**
- Email: preetiup28@gmail.com


