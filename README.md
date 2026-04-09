# Traffic Accident Analysis in Turkey Based on Weather Conditions and Time of Day
---

## 1.Project Overview
People in Turkey spend a large part of their daily lives in traffic. This is mainly because traffic is a common problem across the country and people prefer comfortable ways of transportation. Also, the number of registered vehicles in Turkey increases every year. In this study, we aim to examine the results of driving behavior in Turkey during rainy weather and at night.

## 2.Research Questions and Sub-Questions

### Main Question
- Do weather conditions and time of day affect traffic accidents in Turkey?

### Sub-Questions
- Does rainy weather increase the rate of fatal traffic accidents in Turkey?
- Are traffic accidents that occur at night more likely to result in fatalities compared to daytime accidents?
- Is there a relationship between monthly rainfall levels and the number of traffic accidents?

## 3.Hypotheses
- H1: Fatal traffic accident rates are higher during rainy weather conditions in Turkey.
- H2: Traffic accidents that occur at night have a higher fatality rate than accidents that occur during the day.

## 4. Data Description
| Dataset | Variables | Why used |
|----------|--------------|----------|
| **TÜİK – Monthly Distribution of Fatal and Injury Traffic Accidents, Deaths, and Injuries (2020-2024)** | Traffic accident counts and accident outcomes across Turkey by months | It helps identify seasonal patterns and allows comparison with weather conditions |
| **TÜİK – Fatal and Injury Traffic Accidents, Number of Deaths and Injuries by Daylight Conditions (2020-2024)** | Daylight conditions (day/night), number of accidents, number of deaths, and number of injuries |It helps evaluate whether accidents occurring at night result in higher fatality and injury rates compared to daytime accidents. |
| **Open-Meteo – Historical Forecast API (2020-2024)** | provides monthly rain levels across Turkey | compare whether accident rates are higher during months with higher rain levels. |

## 5. Data Source and Collection
- All datasets are publicly available through the https://veriportali.tuik.gov.tr/ and https://open-meteo.com.
- Data will be collected between 2020 (January 1) and 2024 (December 31)

  
## 6. Methodology 
- First, accident data will be grouped by months, and key variables such as total accidents, number of fatal cases, and number of injuries will be calculated. Then, fatality rates will be computed by dividing the number of fatal accidents by the total number of accidents.
- Weather data, specifically monthly rain levels, will be matched with the corresponding months of accident data. This will allow comparison between rainfall levels and accident severity.
- Line charts and bar charts will help observe trends over months, while simple correlation analysis will be applied to see the relationship between rain and accident rates.
- To analyze the effect of time of day, accident data categorized by daylight conditions (day/night) will be used. Fatality rates for day and night accidents will be calculated and compared.
- In the final stage, simple predictive models may be developed using weather and time-related variables to estimate accident likelihood and severity.

## 7. Expected Results

- It is expected that traffic accident severity will increase during months with higher rain levels. In particular, the rate of fatal accidents is likely to be higher in rainy conditions due to reduced visibility and road safety.
- It is also expected that accidents occurring at night will have a higher fatality rate compared to daytime accidents. This may be due to factors such as lower visibility, driver fatigue, and lower reaction time.
- Additionally, the analysis may show seasonal patterns in accident frequency, with certain months having higher accident rates than others. Overall, the results are expected to reveal a clear relationship between weather conditions, time of day, and accident severity in Turkey.
