# Learning Outcomes Addressed

- Describe how principal component analysis (PCA) is used to augment data analysis
- Apply PCA to reduce the dimensionality of datasets while preserving as much variance as possible
- Apply PCA for practical purposes such as data visualisation, noise reduction, and feature extraction
- Explain the concept of feature engineering and its role in enhancing model performance
- Create new features based on existing ones and apply transformations to improve data quality
- Utilise software tools and libraries for dimensionality reduction, feature scaling, and feature selection

---

# Assignment Instructions

- You must attempt **both given tasks**.
- Each task carries a **maximum of 10 points**, totalling **20 points** for the assignment.
- Each task consists of **sub-tasks/questions** that must be completed as part of your response.
- Ensure **clarity, depth, and relevance** in your answers to maximise your score.

---

# Task 1: PCA on Wine Quality Dataset

In this part of the assignment, you will apply **Principal Component Analysis (PCA)** on the Wine Quality Dataset to understand how dimensionality reduction can preserve key data structures and influence model performance.

You will begin by **standardising the data and performing PCA** to reduce it to a lower-dimensional form. You will then **evaluate the number of components required to retain 90% of the variance**. Finally, you will **compare the performance of a classification model built on original features versus reduced components**.

Dataset:  
`winequality-red.csv`

---

## Preprocessing

- Load the dataset.
- Check for **missing values** and **basic statistics**.
- Standardise all **feature columns** (exclude the target `quality`).

---

## Apply PCA

- Apply **PCA** to the standardised dataset.
- Plot the **explained variance ratio**.
- Plot the **cumulative variance**.
- Identify the **minimum number of components required to retain at least 90% of total variance**.

---

## Visualisation

Create a **2D scatter plot** using the **first two principal components**.

Group wine samples into three quality categories:

- **Low:** quality 3–5  
- **Medium:** quality 6  
- **High:** quality 7–8  

Requirements:

- Colour the data points based on these categories in the scatter plot.

---

## Interpretation

Answer the following reflection questions:

- How many components are needed to retain **90% variance**?
- What do you observe from the **PCA 2D plot**?
- Are there **clear clusters** for wine quality categories?
- What does PCA reveal about **feature correlations or redundancy**?

---

## Questions

1. **How does PCA help identify redundant or less informative features in high-dimensional datasets?**

2. **Why is it important to standardise features before applying PCA, and what could happen if we skip this step?**

---

# Task 2: Feature Selection on Telco Customer Churn Dataset

In this part of the assignment, you will work with the **Telco Customer Churn dataset** to explore how **preprocessing (scaling + encoding)** and **feature selection methods** affect the performance of churn prediction models.

Dataset:  
`WA_Fn-UseC_-Telco-Customer-Churn.csv`

Target column:  
`Churn (Yes/No)`

---

## Preprocessing and Feature Scaling

- Load the dataset and **drop `customerID`**.
- Convert **TotalCharges** to numeric and handle **missing values**.
- Encode categorical columns using **OneHotEncoding**.

Apply the following scalers to numeric features:

- **MinMaxScaler**
- **StandardScaler**
- **RobustScaler**

Create **boxplots for each scaled dataset** and compare:

- Which scaler **handles outliers best**?
- Which scaler **centres values around zero**?

---

## Variance Threshold

Apply: VarianceThreshold(threshold=0.01) to remove low-variance features


Tasks:

- Remove **low-variance features**.
- Report **how many features were removed**.
- List the removed features.
- Discuss whether they seem **informative or redundant**.

---

## SelectKBest and RFE

Apply two feature selection methods:

### SelectKBest

- Use `SelectKBest(chi2)`
- Select the **top 10 features** (after scaling and encoding)

### RFE

- Use `RFE(LogisticRegression)`
- Select the **top 10 features**

Tasks:

- List features selected by **each method**
- Compare the differences
- Explain **why the selected features differ**

---

## LASSO for Feature Selection

- Apply **StandardScaler** on numeric data
- Use **LassoCV**

Tasks:

- Retrieve and visualise **feature coefficients**
- Report features with **non-zero coefficients**
- Discuss how **LASSO handles feature correlation and redundancy**

---

## Final Model Pipeline

Build a **machine learning pipeline** including:

1. **Preprocessing**
   - Imputation
   - Scaling
   - Encoding

2. **Feature Selection**
   - `SelectFromModel(LassoCV)`

3. **Classification**
   - `LogisticRegression`

Evaluate the model using:

- **Accuracy**
- **ROC-AUC**
- **RMSE**
- **MAE**

---

## Discussion Questions

1. **Why is it important to perform both encoding and scaling before applying LASSO or PCA in datasets with mixed data types?**

2. **How do embedded methods like LASSO differ from filter and wrapper feature selection methods?**

---

# Submission Instructions

- Go through the instructions and evaluation rubric to understand expectations.
- Collate all **textual responses in a document file**.

