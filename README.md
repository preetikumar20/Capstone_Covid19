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
 <img width="441" alt="image" src="https://github.com/user-attachments/assets/b1c9b580-c1e8-465f-8faa-37fe19fa7680" />

- **Death Distribution:** Distribution with many days recording low deaths and occasional extreme spikes.
<img width="492" alt="image" src="https://github.com/user-attachments/assets/2b9a907f-a482-4977-b3cf-9fe3a0aba737" />

- **Wave Patterns:** Two major peaks corresponding to the Delta and Omicron variants (2022 and 2023).

 <img width="701" alt="image" src="https://github.com/user-attachments/assets/edcd7a45-f1bb-40a3-8f26-b9644f2fcff9" />


- **Country-specific Trends:** 
  - The USA experienced the highest case count in early 2022.
  - China saw a significant peak in late 2022.

 ![image](https://github.com/user-attachments/assets/299c3552-968c-4cc1-a2ed-827fc7372360)

 
- **Mortality Trends:** 
  - The USA had the highest death toll, followed by Brazil and India.

<img width="960" alt="image" src="https://github.com/user-attachments/assets/8952ee0e-c6e5-492a-b802-d01efe499d47" />



### 3. Model Selection 🤖
We implemented time series forecasting models to predict future COVID-19 cases:
- **ARIMA Model**
- **SARIMA Model**
- **Exog SARIMA Model**
- **Random Forest**
- **XGBoost**
- **LSTM**

### 4. Model Evaluation 📈
Models were evaluated using performance metrics such as MAE and RMSE.
The comparative chart below summarizes the evaluation:

| Model           | MAE        | RMSE       | 
|-----------------|------------|------------|
| ARIMA           | 134,360.86 | 157,527.53 | 
| SARIMA          | 97,100.10  | 128,000.76 | 
| EXOG SARIMA     | 79,852.14  | 93,150.65  | 
| Random Forest   | 68,322.60  | 81,348.77  | 
| XGBoost         | 122,012.04 | 181,259.30 |
| LSTM            | 411905.47  | 93155.53 |   

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
- **Random Forest:** Minimizes MAE more effectively than ARIMA/SARIMA/exog SARIMA.
- **XGBoost:** Underperforms relative to Random Forest; may need additional tuning.
- **LSTM:** Performs poorly, making it worst approach for predicting new COVID-19 cases in the USA.
- 
![image](https://github.com/user-attachments/assets/2847d01b-abe4-48c9-bede-d079e15a8fd6)


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







