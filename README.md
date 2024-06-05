# Credit Risk Analysis

## Deliverables Overview

This project encompasses a comprehensive analysis of credit risk, including data understanding, exploratory data analysis, feature engineering, and model building. The following tasks were completed:

1. **Task 1 - Understanding Credit Risk**
2. **Task 2 - Exploratory Data Analysis (EDA)**
3. **Task 3 - Feature Engineering**
4. **Task 3.1 - Default Estimator and WoE Binning**
5. **Task 4 - Modelling**

---

## Task 1 - Understanding Credit Risk

**Objective:** Understand the concept of Credit Risk

**Key References:**
- [Statistica Sinica](https://www3.stat.sinica.edu.tw/statistica/oldpdf/A28n535.pdf)
- [HKMA](https://www.hkma.gov.hk/media/eng/doc/key-functions/financial-infrastructure/alternative_credit_scoring.pdf)
- [World Bank](https://thedocs.worldbank.org/en/doc/935891585869698451-0130022020/original/CREDITSCORINGAPPROACHESGUIDELINESFINALWEB.pdf)
- [Towards Data Science](https://towardsdatascience.com/how-to-develop-a-credit-risk-model-and-scorecard-91335fc01f03)
- [Corporate Finance Institute](https://corporatefinanceinstitute.com/resources/commercial-lending/credit-risk/)
- [Risk Officer](https://www.risk-officer.com/Credit_Risk.htm)

---

## Task 2 - Exploratory Data Analysis (EDA)

**Objective:** Analyze and understand the structure and key characteristics of the dataset.

**Steps and Findings:**

1. **Overview of the Data:**
   - Inspected the number of rows, columns, and data types.
   - Dataset contains `n` rows and `m` columns.

2. **Summary Statistics:**
   - Calculated mean, median, standard deviation, min, and max for numerical features.

3. **Distribution of Numerical Features:**
   - Visualized using histograms.
   - Identified skewness and potential outliers.

4. **Distribution of Categorical Features:**
   - Visualized using bar plots.
   - Observed the frequency and variability of categories.

5. **Correlation Analysis:**
   - Generated a correlation matrix.
   - Identified strong and weak relationships between numerical features.

6. **Identifying Missing Values:**
   - Checked for missing values.
   - Used appropriate imputation strategies to handle missing data.

7. **Outlier Detection:**
   - Used box plots to identify and analyze outliers.

---

## Task 3 - Feature Engineering

**Objective:** Create new features and prepare the dataset for modeling.

**Steps and Findings:**

1. **Create Aggregate Features:**
   - Total Transaction Amount, Average Transaction Amount, Transaction Count, Standard Deviation of Transaction Amounts were calculated for each customer.

2. **Extract Features:**
   - Transaction Hour, Day, Month, and Year were extracted from the transaction timestamp.

3. **Encode Categorical Variables:**
   - Used One-Hot Encoding and Label Encoding to convert categorical values into numerical format.

4. **Handle Missing Values:**
   - Imputed missing values using mean and median imputation.

5. **Normalize/Standardize Numerical Features:**
   - Applied Min-Max Scaling for normalization and StandardScaler for standardization.

6. **Weight of Evidence (WoE) Binning:**
   - Performed WoE binning to transform categorical variables into numerical values with predictive power.

---

## Task 3.1 - Default Estimator and WoE Binning

**Objective:** Construct a default estimator to classify users as high risk or low risk based on RFMS formalism and perform WoE binning.

**Steps and Findings:**

1. **Construct Default Estimator (Proxy):**
   - Calculated RFMS scores (Recency, Frequency, Monetary) for each customer.
   - Established a boundary to classify users into good (high RFMS score) and bad (low RFMS score) categories.

2. **Assign Good and Bad Labels:**
   - Labeled users as good or bad based on the RFMS score boundary.

3. **Perform WoE Binning:**
   - Conducted WoE binning for categorical variables, transforming them into numerical values that hold significant predictive power.
   - **Results:**
     - Generated WoE and IV values for each category in `ProductCategory`.

---

## Task 4 - Modelling




## Conclusion

This analysis provided a comprehensive approach to understanding credit risk, preparing data for modeling, and building and evaluating predictive models. The results highlight the effectiveness of the models in classifying users as high or low risk based on their transaction behaviors and other features.
