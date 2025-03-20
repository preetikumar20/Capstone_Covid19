# Global COVID-19 Trends and New Case Prediction for the USA 🚀

## Project Overview
This project analyzes, forecasts, and evaluates the spread of COVID-19 using both statistical and machine learning models. By leveraging the WHO COVID-19 dataset, we explore global trends, perform extensive exploratory data analysis (EDA), and implement various forecasting models—including ARIMA, SARIMA, Exog SARIMA, Random Forest, XGBoost, and LSTM—to predict future case counts.

## Repository Structure 📂
- **notebooks/** – Jupyter notebooks for data analysis, modeling, and visualization.
- **slides/** – PowerPoint presentation highlighting key aspects of the project.
- **reports/** – Contains both the initial and final project reports.
- **README.md** – This file, which provides an overview of the project.

## Tools Used 🛠️
- **Programming Language:** Python  
- **Data Analysis:** Pandas, NumPy  
- **Visualization:** Matplotlib, Seaborn, Plotly  
- **Time Series & Machine Learning:**  
  - **Statistical Models:** Statsmodels (ARIMA, SARIMA, Exog SARIMA)  
  - **Machine Learning Models:** Scikit-Learn (Random Forest, XGBoost)  
  - **Deep Learning:** TensorFlow/Keras (LSTM)  
- **Development Environment:** Jupyter Notebook, Colab 
- **Version Control:** Git & GitHub

## Methodology 🔍
### 1. Data Collection
- **Source:** WHO COVID-19 dataset from Kaggle.
- **Content:** Weekly confirmed cases and deaths worldwide.

### 2. Exploratory Data Analysis (EDA) 📊

- **Regional Trends:** Higher case frequencies observed in the EMRO and EURO regions.
- 
  <img width="864" alt="image" src="https://github.com/user-attachments/assets/75bbf961-1231-494b-858f-176c03c7ed66" />
  
- **Death Distribution:** Right-skewed distribution with many days recording low deaths and occasional extreme spikes.

   ![deaths_dist_region](https://github.com/user-attachments/assets/bf1578fe-8bd7-419e-a305-79a0e2f5af4c)

- **Wave Patterns:** Two major peaks corresponding to the Delta and Omicron variants (2022 and 2023).

 ![cases_over_time_global](https://github.com/user-attachments/assets/c5d0fb12-3f84-46bf-9cb7-dc57e1a3bd96)

- **Country-specific Trends:** 
  - The USA experienced the highest case count in early 2022.
  - China saw a significant peak in late 2022.

 ![percentage_deaths_country](https://github.com/user-attachments/assets/52d7f59c-bcc2-47d4-9be0-51b5b42152e6)
 
- **Mortality Trends:** 
  - The USA had the highest death toll, followed by Brazil and India.

  ![deaths_percentage_country](https://github.com/user-attachments/assets/47a77231-4fca-4a09-8aef-253d4f8341d5)

### 3. Model Selection 🤖
We implemented time series forecasting models to predict future COVID-19 cases:
- **ARIMA Model**
- **SARIMA Model**
- **Exog SARIMA Model**
- **Random Forest**
- **XGBoost**
- **LSTM**

### 4. Model Evaluation 📈
Models were evaluated using performance metrics such as MAE, MSE, RMSE, AIC, and BIC. 
The comparative chart below summarizes the evaluation:

| Model           | MAE        | MSE         | RMSE       | AIC      | BIC      |
|-----------------|------------|-------------|------------|----------|----------|
| ARIMA           | 134,360.86 | 2.48e+10    | 157,527.53 | 3380.63  | 3397.55  |
| SARIMA          | 97,100.10  | 1.64e+10    | 128,000.76 | 3462.81  | 3474.15  |
| EXOG SARIMA     | 79,852.14  | 8.67e+9     | 93,150.65  | 3669.55  | 3689.84  |
| Random Forest   | 68,322.60  | 6.6e+9      | 81,348.77  | N/A      | N/A      |
| XGBoost         | 122,012.04 | 3.28e+10    | 181,259.30 | N/A      | N/A      |
| LSTM (Training) | 81,126.04  | 3.43e+10    | 185,258.85 | N/A      | N/A      |
| LSTM (Test)     | **38,242.36**  | **5.6e+7**     | **56,711.65**  | N/A      | N/A      |

## Key Findings 📌
### EDA Insights
- **Regional Analysis:** EMRO and EURO regions show higher frequencies of case counts.
- **Multiple Waves:** Evidence of multiple COVID-19 waves (Delta and Omicron variants).
- **Country Trends:** 
  - The USA recorded the highest number of new cases in early 2022.
  - China saw the highest case count towards the end of 2022.
- **Mortality:** The USA observed the highest death toll, particularly in early 2021 and early 2022; India experienced a surge in mid-2021 due to the Delta variant.

### Modeling Insights
- **SARIMA and EXOG SARIMA:** Provide strong baseline forecasts.
- **Random Forest:** Minimizes MAE more effectively than ARIMA/SARIMA but shows higher RMSE.
- **XGBoost:** Underperforms relative to Random Forest; may need additional tuning.
- **LSTM (Test):** Outperforms all other models, making it the most effective approach for predicting new COVID-19 cases in the USA.
  
  ![image](https://github.com/user-attachments/assets/9e49ff99-375e-4277-8949-0b8356310035)

## Deployment 🚀
- The final forecasting results and insights are documented in the final report.
- Visualizations and model predictions are presented to assist in public health decision-making.
- **Final Notebook:** [Capstone Project Jupyter Notebook](https://github.com/preetikumar20/Capstone_Covid19/blob/a871861f8f05c0c51227f05e58bcdd50e33ce2d5/final_capstone_preetidubey.ipynb)

## Visualizations 🌍

- **World Map of COVID-19 Cases:** Visual representation of case distribution globally.
  ![image](https://github.com/user-attachments/assets/2f58231f-a5cb-4fd4-a280-ade3b31cfa8d)

- **World Map of COVID-19 Deaths:** Visual representation of death distribution globally.
![newplot](https://github.com/user-attachments/assets/bb35cdad-b468-43af-af75-89a5507725b1)

## Link for the final capstone project Jupyter notebook
https://github.com/preetikumar20/Capstone_Covid19/blob/a871861f8f05c0c51227f05e58bcdd50e33ce2d5/final_capstone_preetidubey.ipynb

## Contributors 🙌
- **Preeti Dubey**  
  Email: [preetiup28@gmail.com](mailto:preetiup28@gmail.com)







