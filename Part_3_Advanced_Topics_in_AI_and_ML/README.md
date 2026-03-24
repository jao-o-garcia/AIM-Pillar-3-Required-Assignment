# Learning Outcomes Addressed

- Apply advanced machine learning techniques in specialised areas such as Natural Language Processing (NLP), recommender systems, and time-series analysis
- Integrate multiple advanced machine learning techniques into comprehensive solutions for complex problems
- Design and implement recommender systems using information retrieval and collaborative filtering approaches
- Apply machine learning models to perform NLP tasks such as text classification and sentiment analysis
- Develop and evaluate forecasting models to predict future values based on historical data

---

# Assignment Instructions

- You must attempt **both given tasks**.
- Each task carries a **maximum of 10 points**, totalling **20 points** for the assignment.
- Each task consists of **sub-tasks/questions** that must be completed as part of your response.
- Ensure **clarity, depth, and relevance** in your answers to maximise your score.

---

# Task 1: Time Series Analysis and Forecasting

Dataset: Generate a **synthetic time series with 365 days** and forecast the **next 60 days**.

The generated dataset should include:

- **Linear upward trend**
- **Weekly seasonality** (7-day sinusoidal pattern)
- **Random Gaussian noise**

---

## Data Generation and Visualisation

Objective: Simulate a realistic time series for one year.

Tasks:

- Generate a **time series of 365 points** with:
  - Trend: **linear**
  - Seasonality: **weekly sine wave**
  - Noise: **random normal noise (mean = 0, std = 3)**
- Plot the time series with **proper titles and labelled axes**

Describe:

- Is the **trend visible**?
- How strong is the **weekly pattern**?
- Is the **noise low or high**?

---

## Time Series Decomposition

Objective: Decompose the time series into meaningful components.

Tasks:

- Use **seasonal_decompose()** from `statsmodels`
- Apply both:
  - **Additive model**
  - **Multiplicative model**
- Set `period = 7`

Plot the following components:

- Observed
- Trend
- Seasonal
- Residuals

Compare:

- Which model captures **seasonality better**?
- Are **residuals centred around zero**?

---

## Forecasting Techniques

Objective: Forecast **60 days ahead** using three techniques.

Tasks:

Split the dataset:

- **365 days for training**
- **60 days for testing**

Apply the following forecasting models:

- **7-day Moving Average**
- **Simple Exponential Smoothing (SES)**
- **ARIMA(1,1,1)**

Then:

- Forecast the **next 60 days**
- Plot **actual vs predicted values**

Discussion:

- Which model forecasts **better**?
- Which model **reacts best to recent trends**?

---

## Model Evaluation

Calculate the following evaluation metrics:

- **MAE (Mean Absolute Error)**
- **MSE (Mean Squared Error)**
- **MAPE (Mean Absolute Percentage Error)**

Analyse:

- Which model performs **best**?
- Are there **major deviations**? Why?

---

## Interpretation and Reflection

Answer the following questions:

- Why does **SES flatten after training**?
- What do **decomposition residuals reveal**?
- How does **ARIMA handle seasonality vs Moving Average**?
- What are **real-world use cases** for each forecasting method?

---

## Discussion Questions

1. **Why is decomposing time series important before forecasting?**

2. **What are ARIMA’s limitations in seasonal data scenarios?**

---

# Task 2: Sentiment Analysis Using Rule-Based Tools

Dataset:

`tech_tweets.csv`

This dataset contains tweets related to technology along with sentiment labels.

---

## Data Preprocessing

Objective: Clean and prepare text for sentiment analysis.

Tasks:

- Load the dataset `tech_tweets.csv`
- Clean the tweets by:
  - Converting text to **lowercase**
  - Removing **mentions**
  - Removing **hashtags**
  - Removing **URLs**
  - Removing **punctuation**

(Optional)

- Tokenise text using **NLTK** or **spaCy**

---

## Sentiment Analysis with Rule-Based Tools

Objective: Classify tweet sentiment using rule-based tools.

Use either:

- **TextBlob**
- **VADER**

Tasks:

- Calculate the **polarity score** for each tweet

Label each tweet as:

- **Positive** if polarity > 0
- **Negative** if polarity < 0
- **Neutral** if polarity == 0

---

## Compare with Ground Truth Labels

Objective: Evaluate rule-based predictions against actual labels.

Tasks:

- Compare **predicted sentiment vs sentiment column**

Calculate:

- **Accuracy**
- **Confusion Matrix**

Visualise the confusion matrix using a **Seaborn heatmap**.

---

## Interpretation and Reflection

Answer the following questions:

- How well did the **rule-based method perform**?
- Provide examples of **wrongly predicted tweets**.
- Were there **common issues** (e.g., sarcasm, mixed sentiment)?
- When would you **prefer rule-based methods over ML models**?

---

## Discussion Questions

1. **How do rule-based sentiment tools like TextBlob or VADER work?**

2. **What are the limitations of rule-based sentiment analysis?**

---

# Submission Instructions

- Review the **instructions and evaluation rubric** before submission.
- Collate all **textual responses into a document file**.


