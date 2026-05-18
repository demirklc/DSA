# DSA210 Term Project: IMPACTS OF RAINFALL AND DAY TIME ON TRAFFIC ACCIDENTS
**Student:** Doğukan Demirkılıç

**Term:** Spring 2025-2026

## 1. Introduction
### 1.1 Motivation

Traffic accidents are one of the biggest safety problems around the world. Every year thousand of deaths and injuries occurs due to traffic accidents. Understanding the factors that affect or create accidents are is very important to reduce the number of deaths or injuries. Also this is a important way to improve road safety. 
Among many possible factor, as a person that spends a lot of time in traffic, realizing that people drive more dangereous while raining or during night-time was the main motivation of this project.

### 1.2 Objectives

* Investigating whether rainfall has an effect on traffic accident fatality rates.

* Understanding if accident rate increases while raining or during night-time.

* Comparing daytime and night-time accident fatality rates.

* Identifying yearly and monthly traffic accident trends using data visualization techniques,

* Applying statistical methods such as correlation analysis, t-tests, and linear regression to evaluate the hypotheses.

* Developing machine learning models to see how well selected variables can predict accident fatality rates.


## 2. Data & Methodology

### 2.1 Data Sources

* TÜİK – Monthly Distribution of Fatal and Injury Traffic Accidents, Deaths, and Injuries (2020-2024)

* TÜİK – Fatal and Injury Traffic Accidents, Number of Deaths and Injuries by Daylight Conditions (2020-2024)

* Open-Meteo – Historical Forecast API (2020-2024)

All datasets are publicly available through the https://veriportali.tuik.gov.tr/ and https://open-meteo.com.

Data is collected between 2020 (January 1) and 2024 (December 31)

### 2.2 Data Cleaning

* Columns are renamed as "YEAR" or "ACCIDENTS" to have for readability and consistency.

* Numerical values stored as strings were converted into numeric data types.

* Categorical daylight data was encoded into numerical form for correlation and regression analysis.


## 3. Exploratory Data Analysis

Exploratory Data Analysis was performed to better understand the structure and trends in the dataset before applying statistical tests.

**Average Monthly Rainfall Between 2020 and 2024**

<img width="952" height="541" alt="image" src="https://github.com/user-attachments/assets/88299cfc-e725-4223-9ed0-ea88eb3ab905" />




**Monthly Accident by Year**

<img width="950" height="559" alt="image" src="https://github.com/user-attachments/assets/3b0a82da-ca36-40c2-ac75-75d1273cb545" />



**Combined Average Monthly Rainfall x Accidents by Year**

<img width="1010" height="551" alt="image" src="https://github.com/user-attachments/assets/23a1d4f6-aae3-438a-ad86-f2190a9e50cb" />

**Comparison of Rainfall and Fatality Rate**
<img width="629" height="456" alt="image" src="https://github.com/user-attachments/assets/16833628-bbbb-4889-a5aa-c065c8f3a658" />


**Accidents Seperated DayTime and Nigh-Time**
<img width="1455" height="569" alt="image" src="https://github.com/user-attachments/assets/02e8b191-561e-47b2-86f7-174f3dc1e73b" />

**Comparison of Fatality Rate**
<img width="935" height="542" alt="image" src="https://github.com/user-attachments/assets/ccdb67e6-bedd-4595-9e19-7de91979da89" />

**Comparison of Fatality Rate**
<img width="882" height="543" alt="image" src="https://github.com/user-attachments/assets/a6551e0c-0839-4bbd-8371-b6e50e2c71bb" />


## 4. Hypothesis Testing
In order to evaluate the hypotheses, several statistical analysis methods were applied throughout the project.

**Hypothesis 1**
* Pearson correlation analysis is used to measure the linear relationship between rainfall and fatality rate. A weak negative correlation (-0.26) was found.
* T-test showed that there is no statistically significant difference between high and low rainfall groups (p=0.477 > 0.05).
* Linear regression shows a very weak negative relationship between rainfall and fatality rate. (R^2 = 0.067).
* Spearman correlation indicated a weak negative relationship between rainfall and fatality rate (-0.28).

**Hypothesis 2**
* Pearson correlation shows a positive relationship (0.84).
* Spearman correlation shows a positive relationship (0.88).
* Both Pearson and Spearman correlations show significant positive relationship between night-time and fatality rate.
* T-test applied to see correlation. P = 0.0025 < 0.05 gives a very strong correlation between night-time and fatality rate.
* Also Linear Regression R^2: 0.69, shows that transforming daytime to night-time increases fatality rate.

**Hypothesis Conclusions**

**Hypothesis 1:** The initial hypothesis that rainfall increases fatality rate is not supported by the results. Instead, the analysis suggests a weak negative relationship, indicating that higher rainfall may be associated with slightly lower fatality rates.

**Hypothesis 2:** The graphs and test results are clearly indicated that night-time accidents are significantly more fatal than daytime accidents.

## 5. Machine Learning Analysis
In this part, rainfall and time of day were used together as input features to predict fatality rates. The dataset was split into training and testing sets. Three supervised learning models were applied: Linear Regression, Decision Tree, and Random Forest.
The results showed that all models performed poorly, with negative R^2 scores. This indicates that the selected features are not sufficient to accurately predict fatality rates.


## 6. AI Usage Disclaimer

OpenAI’s ChatGPT was used during the development of this project for guidance, debugging support, code explanation. All analyses and final decisions were made manually.

