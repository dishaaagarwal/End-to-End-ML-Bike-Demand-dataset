# End-to-End-ML-Bike-Demand-dataset
In this repository I have solved the End to End Bike demand dataset using Python and Machine Learning


## Bike Demand-Prediction-Dataset

From the challange hosted at: https://www.kaggle.com/c/bike-sharing-demand/overview


## Problem Statement:

This is a **Regression problem** in which the participants are asked to forecast bike rental demand of Bike sharing program in Washington, D.C based on historical usage patterns in relation with weather, time and other data.

Using these Bike Sharing systems, people rent a bike from one location and return it to a different or same place on need basis. People can rent a bike through membership (mostly regular users) or on demand basis (mostly casual users). This process is controlled by a network of automated kiosk across the city.


## The Data

Variable | Description
----------|--------------

- datetime |   date and hour in "mm/dd/yyyy hh:mm" format

- season   |  Four categories-> 1 = spring, 2 = summer, 3 = fall, 4 = winter

- holiday   | whether the day is a holiday or not (1/0)

- workingday | whether the day is neither a weekend nor holiday (1/0)

- weather   | Four Categories of weather

            1-> Clear, Few clouds, Partly cloudy, Partly cloudy
            2-> Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
            3-> Light Snow and Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
            4-> Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
            
- temp      | hourly temperature in Celsius

- atemp     | "feels like" temperature in Celsius

- humidity  | relative humidity

- windspeed | wind speed


## Table of Content

- **Hypothesis Testing**


1. Most people might tend to rent a bike during morning for going to office or after office hours to return home.

2. Users might rent a bike during weehdays instead of weekends and holidays.

3. In India ,temperature and negative correlation with the rentals, but it might be a diffrent case in Washington.

4. Users will preferr to rent a bike when humidity is low.

5. The demand of bikes will be low during rainy days.

6. It is expected that registered users are more than casual users.

7. Traffic can be positively correlated with Bike demand. Higher traffic may force people to use bike as compared to other road transport medium like car, taxi etc.


- **EDA**

![](/images/Univariate_1.png)
![](/images/Univariate_2.png)
![](/images/Multivariate_1.png)
![](/images/Multivariate_2.png)
![](/images/Multivariate_3.png)

- **Data Cleaning**

- **Feature Engineering**

![](/images/Feature_eng_1.png)


- **Model Building**

For this I have build a 2 Pipelines one for testing Regression algorithms and another for Ensembled Methods. I have used Cross Validation alogside to compare across models.
For Evaluation I have used **R2** metric.

![](/images/model_pipeline.png)
![](/images/ensembled_pipeline.png)



- **Making Final Submission**

For final prediction I have used Random Forest  with evaluation metric as **RMSLE**=0.2
