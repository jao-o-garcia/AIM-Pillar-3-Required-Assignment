# Dimensionality Reduction & Feature Engineering Assignment Rubric

## Task 1: PCA on Wine Quality Dataset


| Task                         | Criteria for Full Points                                                                                                                                             | Partial Points                                                                  | No Points                                                     |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| **1. Data Preprocessing**    | Dataset loaded correctly, missing values handled, and feature columns properly standardised **(2 points)**                                                           | Minor preprocessing issues or incomplete standardisation **(1 point)**          | No preprocessing or incorrect handling of data **(0 points)** |
| **2. PCA Application**       | PCA correctly applied, explained variance ratio and cumulative variance plotted, and the number of components for **90% variance** clearly identified **(2 points)** | PCA applied but variance plots or interpretation unclear **(1 point)**          | PCA not applied or implemented incorrectly **(0 points)**     |
| **3. Visualisation**         | Clear **2D scatter plot using first two principal components**, with wine quality categories (Low, Medium, High) clearly distinguished **(2 points)**                | Scatter plot created but categories poorly represented or unclear **(1 point)** | No visualisation or incorrect plot **(0 points)**             |
| **4. Interpretation of PCA** | Insightful interpretation of PCA results including variance retention, cluster patterns, and feature relationships **(2 points)**                                    | Basic interpretation provided but lacking depth or clarity **(1 point)**        | No interpretation or incorrect conclusions **(0 points)**     |
| **5. Question Responses**    | Clear explanation of **PCA’s role in identifying redundant features** and the **importance of feature standardisation** **(2 points)**                               | Partial explanation with limited understanding **(1 point)**                    | Missing or incorrect explanations **(0 points)**              |


---

# Task 2: Feature Selection on Telco Churn Dataset


| Task                           | Criteria for Full Points                                                                                                                                                                                     | Partial Points                                                               | No Points                                                     |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------- | ------------------------------------------------------------- |
| **1. Preprocessing & Scaling** | Dataset cleaned, `customerID` removed, `TotalCharges` converted to numeric, categorical features encoded, and all **three scalers (MinMax, Standard, Robust)** applied with boxplot comparison **(1 point)** | Partial preprocessing or missing one scaler **(0.5 point)**                  | No preprocessing or scaling applied **(0 points)**            |
| **2. Variance Threshold**      | Low-variance features removed using `VarianceThreshold(0.01)` and results discussed with justification **(1 point)**                                                                                         | Features removed but discussion unclear or incomplete **(0.5 point)**        | No thresholding or incorrect implementation **(0 points)**    |
| **3. SelectKBest & RFE**       | Both **SelectKBest(chi2)** and **RFE(LogisticRegression)** applied correctly; top features listed and differences clearly explained **(2 points)**                                                           | Methods applied but comparison unclear or incomplete **(1 point)**           | Methods not applied or implemented incorrectly **(0 points)** |
| **4. LASSO Feature Selection** | **LassoCV applied**, coefficients visualised, and non-zero features clearly interpreted **(2 points)**                                                                                                       | LASSO applied but visualisation or interpretation unclear **(1 point)**      | LASSO not applied or implemented incorrectly **(0 points)**   |
| **5. Final Model Pipeline**    | Complete pipeline implemented including preprocessing, feature selection (`SelectFromModel(LassoCV)`), and **LogisticRegression**, evaluated with **Accuracy, ROC-AUC, RMSE, MAE** **(2 points)**            | Pipeline built but missing steps or limited evaluation metrics **(1 point)** | Pipeline missing or incorrectly implemented **(0 points)**    |
| **6. Question Responses**      | Clear explanation of **why encoding and scaling are necessary** and comparison of **embedded vs filter vs wrapper feature selection methods** **(2 points)**                                                 | Partial explanation or shallow comparison **(1 point)**                      | Missing or incorrect explanations **(0 points)**              |


