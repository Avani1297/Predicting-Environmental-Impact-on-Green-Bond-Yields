# Predicting-Environmental-Impact-on-Green-Bond-Yields

## Introduction
The primary objective of this project is to enhance investment strategies for green bonds by analyzing environmental risks. By integrating diverse data sources, such as weather data, natural disaster occurrences, and cloud coverage estimates, the project aims to identify how these environmental factors impact green bond performance. This analysis enables investors to make informed decisions, manage associated risks, and optimize their portfolios for better financial returns.

## Implementation
### Data Collection
#### Weather Data: 
Collected using Visual Crossing API, including variables such as temperature, precipitation, humidity, and more.
#### Bond Data: 
Historical price data for the iShares Global Green Bond ETF (BGRN).
#### Satellite Image Data: 
Sourced from NASA, includes the count of natural calamities observed.

### Feature Extraction and Engineering
#### Template Matching using OpenCV: 
Employed to detect and extract specific environmental features from satellite images.
##### Data Preprocessing: 
Included handling data types, removing outliers, and aligning timestamps.
#### Models Used
###### 1. Linear Regression
###### 2. Decision Tree
###### 3. Random Forest
###### 4. XG Boost
###### 5. Neural Network
The models were tested with and without enriched features such as natural disaster occurrences and cloud coverage percentages.

#### Key Techniques
Cloud Cover Percentage Calculation: Used grayscale conversion and binary thresholding to estimate cloud coverage from satellite images.
Template Matching for Natural Disasters: Identified occurrences of natural disasters by matching smaller image segments to predefined templates.

## Results
#### Random Forest Model: 
Achieved the highest R-squared value of 45% when enriched features were included.
#### Cloud Coverage: 
Emerged as the second most important feature in the analysis.
#### Model Performance: 
Improved significantly with the inclusion of features derived from image processing techniques.
### Key Observations
###### 1. Random Forest is the best-performing model with an R-squared value of 45%.
###### 2. Enhanced Features: Models including natural disasters and cloud cover % features outperformed those without these enriched features.
###### 3. Importance of Image Processing: Cloud cover was identified as the second most important feature, indicating the value of image processing in enhancing model performance.
