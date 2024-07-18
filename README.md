# Repository1
 # REVIEW PAPER: QUANTITATIVE CORRELATION BETWEEN US FEDERAL RESERVE INTEREST 
RATES AND INDIAN RBI RATES (2000-2023) 
Survesh Bajpai (NISM-PGP04078)       
+91-7898696623 
Surveshb-pgp-2024-25@nism.ac.in 
Date – 05/07/2024 
## ABSTRACT 
This paper examines the quantitative correlation between the interest rates set by the US Federal Reserve (Fed) 
and the Reserve Bank of India (RBI) over the period from 2000 to 2023. Using historical data, we aim to establish 
the extent to which the Fed's monetary policy influences RBI's rate decisions. The analysis reveals a significant 
correlation coefficient of 0.682451, indicating a moderate positive relationship between the two sets of interest 
rates. 
## INTRODUCTION 
Interest rates are a crucial tool for central banks in managing economic stability. The US Federal Reserve and the 
Reserve Bank of India use their respective interest rates to influence economic activity, inflation, and employment. 
This paper investigates the relationship between the Fed funds rate and the RBI repo rate to understand how the 
monetary policy in one of the world's largest economies affects a major emerging market economy. 
## METHODOLOGY 
### DATA COLLECTION 
The study uses monthly interest rate data from January 2000 to December 2023. The Fed funds rate data is 
sourced from the Federal Reserve, while the RBI repo rate data is obtained from the Reserve Bank of India's official 
records.  
### STATISTICAL TOOLS 
1. *Correlation Analysis*: Pearson correlation coefficient is used to measure the linear relationship between the 
two interest rates. 
2. *Time Series Analysis*: The data is plotted to visualize trends and co-movements over the specified period. 
3. *Regression Analysis*: Simple linear regression is performed to quantify the impact of the Fed funds rate on the 
RBI repo rate. 
### QUANTITATIVE ANALYSIS 
Using the real-world data provided from FRED and RBI websites, the Pearson correlation coefficient between the 
Fed funds rate and the RBI repo rate is calculated to be 0.682451. This value indicates a moderate positive 
correlation, suggesting that changes in the Fed funds rate are associated with changes in the RBI repo rate in the 
same direction. 
![image](https://github.com/user-attachments/assets/03455b52-f4f1-4c24-93b9-0fa7830e464a)
![image](https://github.com/user-attachments/assets/e2270072-c796-4301-8390-24cd3dd2d06f)
FEDFUNDS Descriptive Stats	
	
Mean	0.677716142
Standard Error	0.237316329
Median	1.08
Mode	0.08
Standard Deviation	2.095921066
Sample Variance	4.392885115
Kurtosis	-0.089497337
Skewness	1.100932968
Range	6.49
Minimum	0.05
Maximum	6.54
Sum	141.9
Count	78
Confidence Level(95.0%)	0.472557183
Coeff. Of variation	309.2623792
	
	
RBIRATES Descriptive Stats	
	
Mean	6.259151798
Standard Error	0.221764731
Median	6.25
Mode	4
Standard Deviation	1.958573069
Sample Variance	3.836008467
Kurtosis	1.74331775
Skewness	1.043243389
Range	9.5
Minimum	4
Maximum	13.5
Sum	508.952
Count	78
Confidence Level(95.0%)	0.441589995
Coeff. Of variation	31.29134957
	
	
Correlation = 	0.682451292
Covariance (RBI vs FED)	2.801472488
Variance (FED)	4.392885115
Sensitivity=Beta(Cov/Var)	0.637729514
	
SUMMARY OUTPUT	
	
Regression Statistics	
Multiple R	0.692152996
R Square	0.479075769
Adjusted R Square	0.472130113
Standard Error	1.432324177
Observations	77
![image](https://github.com/user-attachments/assets/7c2df257-272b-4878-a85a-d1c269a4fd20)

Beta (slope): 0.6377295135763537
Alpha (intercept): 5.364848487480967
Standard Error: 0.07834918523751774
p-value: 5.9493265909120915e-12

Now Building 4 LSTM deep learning model to predict the future RBI rates -

1) A model-1 that takes 60 years historic fedrates to predict future rates till 2042.
2) A model-2 takes the predicted fed rate data from model-1 as input and predicts the RBI rates till 2042.
3) A model-3 takes the predicted RBI rate data from model-2 as input and predicts the NIFTY index price action till 2042.
4) A model-4 takes the predicted NIFTY    data from model-3 as input and predicts the Mutual Fund price action till 2042.

Lets start -

1) A model-1 that takes 60 years historic fedrates to predict future rates till 2042.
   
Building LSTM model to predict future FED funds rates by training last 60 years of historic Fed fund rates -

Training data -
![image](https://github.com/user-attachments/assets/f3929433-ae52-49a3-ac4d-3135c207ca47)

Training prediction -
![image](https://github.com/user-attachments/assets/9791d963-48b7-4280-8aba-5746ab9c7415)


Testing Prediction of the Future Fed fund rates till 2042 -
![image](https://github.com/user-attachments/assets/4489b34a-1d0e-4419-b722-036c9e06690a)

Model-1 3d Graphical representation -
![image](https://github.com/user-attachments/assets/5e88dc99-5f29-4e0c-9e96-ad5468de470c)



2) A model-2 takes the predicted fed rate data from model-1 as input and predicts the RBI rates till 2042.

Training data -
![image](https://github.com/user-attachments/assets/f81f91f4-7c01-4ccf-a84a-86cc30194a02)

Training prediction -
![image](https://github.com/user-attachments/assets/3d48bb7b-d79b-4156-a172-d7ee4f4ef73c)
![image](https://github.com/user-attachments/assets/c8a63e68-b6ee-4546-b7a4-bd4e2a5747ae)


This Future fed rate data till 2042 will be our testing Data to predict RBI rates till 2042 -

Testing prediction - 
![image](https://github.com/user-attachments/assets/ad1eb8e1-8434-4b97-9290-7758bfca5bfb)

Model-2 3d Graphical representation -
![image](https://github.com/user-attachments/assets/feb144bb-7129-4bf8-af6d-5ac387a0181c)

3) A model-3 takes the predicted RBI rate data from model-2 as input and predicts the NIFTY index price action till 2042.

Model-3 3d graphical representation -
![image](https://github.com/user-attachments/assets/7d63802e-6088-4069-82f9-8b5cec901b5f)


4) A model-4 takes the predicted NIFTY    data from model-3 as input and predicts the Mutual Fund price action till 2042

Model-4 3d graphical representation -
![image](https://github.com/user-attachments/assets/7d63802e-6088-4069-82f9-8b5cec901b5f)


## RESULTS AND DISCUSSION 
### CORRELATION ANALYSIS 
The correlation coefficient of 0.682451 demonstrates a significant relationship between the two interest rates. 
While not implying causation, this positive correlation indicates that higher Fed rates tend to be associated with 
higher RBI rates and vice versa. 
### TIME SERIES ANALYSIS 
The time series plots of the Fed funds rate and the RBI repo rate exhibit similar trends, particularly during periods 
of global financial crises and economic recoveries. This visual inspection supports the quantitative finding of a 
positive correlation. 
### REGRESSION ANALYSIS 
The regression model, where the RBI repo rate is the dependent variable and the Fed funds rate is the 
independent variable, shows a statistically significant positive slope. This suggests that a one-unit increase in the 
Fed funds rate corresponds to an increase in the RBI repo rate, reinforcing the correlation analysis results. 
### IMPLICATIONS 
The moderate correlation between the Fed and RBI rates highlights the interconnectedness of global financial 
markets. As the US economy influences global capital flows and investor sentiment, the RBI may adjust its rates in 
response to Fed policies to manage inflation, exchange rates, and economic growth. 
## CONCLUSION 
This study finds a moderate positive correlation of 0.682451 between the US Fed funds rate and the Indian RBI 
repo rate from 2000 to 2023. The results underscore the importance of considering global monetary policy trends 
in national economic planning. Future research could delve deeper into causation factors and the influence of 
other macroeconomic variables on this relationship. 
## REFERENCES 
Several studies have explored the influence of US Fed rates on global monetary policies, including India's. The 
following four papers are instrumental in understanding the causality between Fed funds rates and RBI repo rates: 
1. *Paper 1*: [Sewak Pradhan and G Raghavender Raju, 2020,Monetary Policy Shocks and Macroeconomic 
Variables: Evidence from India]  
2. *Paper 2*: [Amalendu Bhunia , 2016, How Inflation and Interest Rates Are Related to Economic Growth? A Case 
of India] 
3. *Paper 3*: [Anshu Grewal, 2013, Impact of Rupee- Dollar Fluctuations on Indian Economy: Challenges for Rbi & 
Indian Government] 
4. *Paper 4*: [Ila Patnaik and Ajay Shah, 2003, Interest-rate risk in the Indian banking system] - Federal Reserve Economic Data (FRED), Federal Reserve Bank of St. Louis. - Reserve Bank of India (RBI) official records and publications 
## ANNEXURE 
