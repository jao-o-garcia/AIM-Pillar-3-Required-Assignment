# Advanced Topics in AI/ML Assignment Rubric

## Task 1: Time Series Analysis and Forecasting


| Task | Criteria for Full Points | Partial Points | No Points |
|-----|-----|-----|-----|
| **1. Data Generation & Visualisation** | Time series correctly generated with **trend, weekly seasonality, and Gaussian noise**. Plot clearly labelled and interpretation provided **(1 point)** | Time series generated but plot unclear or interpretation weak **(0.5 point)** | No time series generated or incorrect implementation **(0 points)** |
| **2. Time Series Decomposition** | Both **additive and multiplicative decomposition** applied using `seasonal_decompose(period=7)` with proper comparison of components **(1 point)** | Only one decomposition model used or comparison unclear **(0.5 point)** | No decomposition or incorrect method used **(0 points)** |
| **3. Forecasting Techniques** | All three forecasting models (**7-day Moving Average, SES, ARIMA(1,1,1)**) implemented correctly and plotted with comparison **(2 points)** | Models implemented but comparison unclear or incomplete **(1 point)** | Forecasting not implemented or incorrect **(0 points)** |
| **4. Model Evaluation** | **MAE, MSE, and MAPE** calculated and interpreted correctly; best model identified with reasoning **(2 points)** | Metrics calculated but interpretation unclear **(1 point)** | No evaluation or incorrect metrics **(0 points)** |
| **5. Interpretation & Reflection** | All reflection questions answered clearly with meaningful analysis of forecasting behaviour **(2 points)** | Answers provided but lacking depth or clarity **(1 point)** | No interpretation or incorrect explanations **(0 points)** |
| **6. Question Responses** | Clear explanation of **time series decomposition importance** and **ARIMA limitations for seasonal data** **(2 points)** | Partial explanation or vague discussion **(1 point)** | No explanation or incorrect concepts **(0 points)** |


---

# Task 2: Sentiment Analysis Using Rule-Based Tools


| Task | Criteria for Full Points | Partial Points | No Points |
|-----|-----|-----|-----|
| **1. Data Preprocessing** | Tweets thoroughly cleaned (**lowercase, remove mentions, hashtags, URLs, punctuation**) with optional tokenisation **(2 points)** | Cleaning performed but missing some preprocessing steps **(1 point)** | No cleaning or incorrect preprocessing **(0 points)** |
| **2. Sentiment Analysis** | Rule-based tool (**TextBlob or VADER**) applied correctly; polarity scores calculated and labelled **(2 points)** | Tool applied but scoring or labelling unclear **(1 point)** | Sentiment analysis not implemented or incorrect **(0 points)** |
| **3. Comparison with Ground Truth** | Predicted sentiment compared with actual labels; **accuracy and confusion matrix** calculated and visualised **(2 points)** | Metrics calculated but visualisation or interpretation unclear **(1 point)** | No comparison or incorrect metrics **(0 points)** |
| **4. Interpretation & Reflection** | Examples of misclassified tweets provided; common issues such as **sarcasm or mixed sentiment** discussed **(2 points)** | Some examples provided but discussion limited **(1 point)** | No interpretation or incorrect analysis **(0 points)** |
| **5. Question Responses** | Clear explanation of **how rule-based sentiment tools work** and their **limitations** **(2 points)** | Partial explanation with limited detail **(1 point)** | Missing or incorrect explanations **(0 points)** |