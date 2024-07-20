# RESEARCH-REVIEW PAPER: QUANTITATIVE Deep Learning Predictive Modelling of US FEDERAL RESERVE INTEREST RATES, INDIAN RBI REPO RATES, NIFTY INDEX, and Mutual Funds

**Survesh Bajpai (NISM-PGP04078)**  
Research Student, NISM. Research & Analysis wing of SEBI.  
+91-7898696623  
Surveshb-pgp-2024-25@nism.ac.in  
Date – 05/07/2024

## ABSTRACT
This paper presents a comprehensive study on the quantitative modeling and prediction of macroeconomic variables and their impact on microeconomic indicators. Using deep learning techniques, we build four LSTM models to predict future values of US Federal Reserve interest rates (Fed rates), Indian Reserve Bank repo rates (RBI rates), NIFTY index, and mutual fund performance. The study demonstrates a successful mapping of macroeconomic movements to microeconomic outcomes, providing predictions up to 2042 based on historical data.

## INTRODUCTION
Interest rates are a crucial tool for central banks in managing economic stability. The US Federal Reserve and the Reserve Bank of India use their respective interest rates to influence economic activity, inflation, and employment. This paper extends the analysis beyond the correlation between the Fed funds rate and the RBI repo rate to predict the future impact of these rates on the NIFTY index and mutual fund performance, demonstrating the interconnectedness of global and local financial markets.

## METHODOLOGY

### DATA COLLECTION AND MANIPULATION
The study uses extensive historical data to train the predictive models:
- **Fed Funds Rate:** Monthly data from January 1960 to December 2023 sourced from the Federal Reserve.
- **RBI Repo Rate:** Data from the Reserve Bank of India's official records.
- **NIFTY Index:** Historical price data.
- **Mutual Funds:** Historical price data.

### STATISTICAL TOOLS
- **Correlation Analysis:** Pearson correlation coefficient to measure the linear relationship between interest rates.
- **Time Series Analysis:** Visualization of trends and co-movements over the specified period.
- **Regression Analysis:** Quantification of the impact of Fed funds rate on RBI repo rate.
- **LSTM Models:** Four LSTM models for predictive analysis.

## QUANTITATIVE ANALYSIS

### Correlation and Regression Analysis
- **Correlation Coefficient:** 0.682451 between Fed funds rate and RBI repo rate, indicating a moderate positive correlation.
- **Regression Statistics:**
  - Multiple R: 0.692152996
  - R Square: 0.479075769
  - Adjusted R Square: 0.472130113
  - Standard Error: 1.432324177
  - Beta (slope): 0.637729514
  - Alpha (intercept): 5.364848487
  - p-value: 5.9493265909120915e-12

### LSTM Predictive Models

#### Model-1: Predicting Future Fed Rates
- **Objective:** Predict future Fed rates till 2042 using 60 years of historic data.
- **Training Data:** Historic Fed fund rates.
- **Results:** Predictions for future Fed rates till 2042.

#### Model-2: Predicting RBI Rates Using Model-1 Output
- **Objective:** Use predicted Fed rates from Model-1 to predict RBI rates till 2042.
- **Training Data:** Predicted Fed rates from Model-1.
- **Results:** Predictions for future RBI rates till 2042.

#### Model-3: Predicting NIFTY Index Price Action Using Model-2 Output
- **Objective:** Use predicted RBI rates from Model-2 to predict NIFTY index price action till 2042.
- **Training Data:** Predicted RBI rates from Model-2.
- **Results:** Predictions for NIFTY index price action till 2042.

#### Model-4: Predicting Mutual Fund Price Action Using Model-3 Output
- **Objective:** Use predicted NIFTY data from Model-3 to predict Mutual Fund price action till 2042.
- **Training Data:** Predicted NIFTY index data from Model-3.
- **Results:** Predictions for Mutual Fund price action till 2042.

## RESULTS AND DISCUSSION

### CORRELATION ANALYSIS
The correlation coefficient of 0.682451 demonstrates a significant relationship between the two interest rates. This positive correlation indicates that higher Fed rates tend to be associated with higher RBI rates and vice versa.

### TIME SERIES ANALYSIS
The time series plots of the Fed funds rate and the RBI repo rate exhibit similar trends, particularly during periods of global financial crises and economic recoveries. This visual inspection supports the quantitative finding of a positive correlation.

![image](https://github.com/user-attachments/assets/03455b52-f4f1-4c24-93b9-0fa7830e464a)
![image](https://github.com/user-attachments/assets/e2270072-c796-4301-8390-24cd3dd2d06f)

### REGRESSION ANALYSIS
The regression model shows a statistically significant positive slope, suggesting that an increase in the Fed funds rate corresponds to an increase in the RBI repo rate.

### PREDICTIVE MODELING RESULTS

#### Model-1 Predictions
- **Training Data Visualization:**
  ![image](https://github.com/user-attachments/assets/f3929433-ae52-49a3-ac4d-3135c207ca47)
  ![image](https://github.com/user-attachments/assets/9791d963-48b7-4280-8aba-5746ab9c7415)
- **Testing Data Predictions:**
  ![image](https://github.com/user-attachments/assets/4489b34a-1d0e-4419-b722-036c9e06690a)
- **Graphical Representation:**
  ![image](https://github.com/user-attachments/assets/5e88dc99-5f29-4e0c-9e96-ad5468de470c)

#### Model-2 Predictions
- **Training Data Visualization:**
  ![image](https://github.com/user-attachments/assets/f81f91f4-7c01-4ccf-a84a-86cc30194a02)
  ![image](https://github.com/user-attachments/assets/3d48bb7b-d79b-4156-a172-d7ee4f4ef73c)
  ![image](https://github.com/user-attachments/assets/c8a63e68-b6ee-4546-b7a4-bd4e2a5747ae)
- **Testing Data Predictions:**
  ![image](https://github.com/user-attachments/assets/ad1eb8e1-8434-4b97-9290-7758bfca5bfb)
- **Graphical Representation:**
  ![image](https://github.com/user-attachments/assets/feb144bb-7129-4bf8-af6d-5ac387a0181c)

#### Model-3 Predictions
- **Graphical Representation:**
  ![image](https://github.com/user-attachments/assets/7d63802e-6088-4069-82f9-8b5cec901b5f)

#### Model-4 Predictions

- **Training Data Visualization:**
  ![image](https://github.com/user-attachments/assets/53ff8d6d-6a24-46f7-aa3a-82ab1e2a4afb)
  ![image](https://github.com/user-attachments/assets/6fb4207b-a33a-4ae9-b1a2-b4ea2512b359)
  ![image](https://github.com/user-attachments/assets/2f0fbba5-60d8-49ec-8231-f35f972ef0d2)
  ![image](https://github.com/user-attachments/assets/625f8780-22f7-4440-a36f-b6403162373a)


- **Testing Data Predictions:**
![image](https://github.com/user-attachments/assets/f77672a9-8631-454b-885f-eed3d43dd0d9)


- **Graphical Representation:**
 ![image](https://github.com/user-attachments/assets/0cc03733-f162-4d35-80b1-0fadc45eea4e)


### IMPLICATIONS
The study highlights the interconnectedness of global financial markets, showing how changes in the US Fed rates can influence Indian economic indicators. The successful prediction of macroeconomic variables down to microeconomic outcomes like mutual fund performance underscores the importance of considering global monetary policies in national economic planning.

## CONCLUSION
This study demonstrates a successful mapping of macroeconomic movements to microeconomic outcomes through deep learning predictive models. The moderate positive correlation between US Fed funds rate and Indian RBI repo rate is quantified, and the predictive modeling extends the analysis to forecast NIFTY index and mutual fund performance till 2042. Future research could explore causation factors and other macroeconomic variables influencing this relationship.

## REFERENCES
Several studies have explored the influence of US Fed rates on global monetary policies, including India's. The following four papers are instrumental in understanding the causality between Fed funds rates and RBI repo rates:
1. Sewak Pradhan and G Raghavender Raju, 2020, "Monetary Policy Shocks and Macroeconomic Variables: Evidence from India"
2. Amalendu Bhunia, 2016, "How Inflation and Interest Rates Are Related to Economic Growth? A Case of India"
3. Anshu Grewal, 2013, "Impact of Rupee-Dollar Fluctuations on Indian Economy: Challenges for RBI & Indian Government"
4. Ila Patnaik and Ajay Shah, 2003, "Interest-rate risk in the Indian banking system"

**Data Sources:**
- Federal Reserve Economic Data (FRED), Federal Reserve Bank of St. Louis.
- Reserve Bank of India (RBI) official records and publications.

---

This version maintains the necessary formatting for headings and subheadings while retaining the provided image links and content.
