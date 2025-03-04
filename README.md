# Exploring Global COVID-19 Trends and Predicting New Cases in the USA

## Project Overview
This project aims to analyze, forecast, and evaluate the spread of COVID-19 using statistical and machine learning models. We utilize the WHO COVID-19 dataset to explore trends, conduct exploratory data analysis (EDA), and implement forecasting models such as ARIMA and SARIMA to predict case counts.

## Repository Structure
- **notebooks/** – Jupyter notebooks used for data analysis, modeling, and visualization.
- **reports/** – Final report.
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

### 4. Model Evaluation
#### ARIMA Model:
- **Mean Absolute Error (MAE):** 134,360.85
- **Mean Squared Error (MSE):** 2.48 × 10¹⁰
- **Root Mean Squared Error (RMSE):** 157,527.53
- **AIC:** 3380.63, **BIC:** 3397.55

#### SARIMA Model:
- **Mean Absolute Error (MAE):** 97,100.10
- **Mean Squared Error (MSE):** 1.64 × 10¹⁰
- **Root Mean Squared Error (RMSE):** 128,000.76
- **AIC:** 3462.81, **BIC:** 3474.15

SARIMA outperformed ARIMA with lower error values, making it a better choice for forecasting.

## Key Findings
- COVID-19 cases exhibited seasonal trends with multiple peaks due to variant outbreaks.
- Public health interventions and vaccinations significantly reduced cases after major waves.
- SARIMA provided better predictive performance than ARIMA.

## Deployment
- The final forecasting results and insights were delivered as a structured report.
- Visualizations and predictions were presented to aid decision-making in public health.

## Link for the Jupyter notebook

## Contributors
- **Preeti Dubey**


