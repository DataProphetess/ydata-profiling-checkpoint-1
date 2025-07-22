🩺 Diabetes Dataset Analysis and Prediction

📌 Project Overview

This project focuses on analyzing the Pima Indians Diabetes Dataset, which contains medical and demographic information relevant to diabetes diagnosis. The aim is to explore the dataset in detail, uncover key patterns and correlations, identify data quality issues (such as missing values or outliers), and lay the groundwork for building a predictive model.

By leveraging Pandas for basic data exploration and YData Profiling for in-depth analysis, this project provides a comprehensive understanding of the dataset’s structure, challenges, and insights. The final goal is to extract valuable information that can guide future machine learning models for diabetes prediction.

📂 Dataset Description

The dataset includes 768 records with 8 input features and 1 binary outcome:

Column	Description

Pregnancies	Number of times the patient was pregnant
Glucose	Plasma glucose concentration (2 hours in an oral glucose tolerance test)
BloodPressure	Diastolic blood pressure (mm Hg)
SkinThickness	Triceps skinfold thickness (mm)
Insulin	2-Hour serum insulin (mu U/ml)
BMI	Body Mass Index (weight in kg/(height in m)^2)
DiabetesPedigreeFunction	Genetic predisposition to diabetes
Age	Age of the patient (years)
Outcome	Diabetes diagnosis outcome (0 = No, 1 = Yes).

🔍 Step-by-Step Process

✅ Step 1: Data Exploration with Pandas

Loaded the dataset using pandas.read_csv().

Displayed structure and metadata using .info(), including column names, data types, and memory usage.

Checked for missing values and invalid zero entries in critical columns like Glucose, Insulin, BMI, etc.

Used .describe() to generate summary statistics (mean, min, max, quartiles) and detect unrealistic values that may need imputation.

✅ Step 2: In-Depth Analysis with YData Profiling

Generated an automated profiling report using the ydata-profiling library.

The report included:

Detailed column descriptions

Distributions of all numerical features

Correlation matrix showing relationships between variables

Automatic detection of missing values and outliers

Highlighted key observations, such as:

Strong correlation between glucose levels and diabetes outcomes

Missing or zero values in Insulin, SkinThickness, and BMI

Impact of age and BMI on diabetes prediction

🧾 Summary of Findings

Glucose is the most predictive variable — higher levels are strongly associated with positive diabetes diagnoses.

BMI and Age also contribute significantly to diabetes risk.

Multiple columns (e.g., Insulin, SkinThickness, BMI, BloodPressure) contain zero values, which likely indicate missing data.

Detected several outliers, especially in Insulin, which may distort model accuracy if not treated.

The data is skewed in certain features and requires scaling and imputation before modeling.
