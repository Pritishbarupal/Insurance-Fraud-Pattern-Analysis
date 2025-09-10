# Insurance-Fraud-Pattern-Analysis

## 📈 Project Overview
This project is an in-depth **Exploratory Data Analysis (EDA)** of a car insurance dataset.  
The primary goal is to identify the **key factors and demographic profiles** associated with a higher likelihood of a policyholder filing a claim.  

Using Python libraries such as **Pandas**, **Matplotlib**, and **Seaborn**, this analysis cleans, processes, and visualizes the data to uncover **actionable insights** that could help an insurance company in **risk assessment and fraud detection**.

- **Dataset:** `car_insurance_claim.csv`  
- **Technologies:** Python, Pandas, Seaborn, Matplotlib, Jupyter Notebook  

---

## Key Questions Explored
The analysis was guided by several business questions:  
1. What is the impact of a driver's past driving record on filing a claim?  
2. Does the primary use of the vehicle (Commercial vs. Private) affect claim frequency?  
3. Is there a relationship between a car's value and the amount claimed?  
4. Do certain occupations have a higher tendency to file claims?  
5. How does a policyholder's income level correlate with filing a claim?  
6. What is the relationship between education level and claim rates?  
7. What are the overall correlations between different numerical features in the dataset?  

---

## Dataset Columns Explained
The dataset contains attributes of the policyholder and their vehicle.  

- **ID** – Unique identifier for each policyholder  
- **KIDSDRIV** – Number of children of driving age  
- **BIRTH / AGE** – Birthdate and age of the policyholder  
- **HOMEKIDS** – Number of children living at home  
- **YOJ** – Years on Job (current employment duration)  
- **INCOME** – Annual income  
- **PARENT1** – Single parent indicator  
- **HOME_VAL** – Value of the policyholder's home  
- **MSTATUS** – Marital status (`Yes` for married)  
- **GENDER** – Gender of the policyholder  
- **EDUCATION** – Highest education level  
- **OCCUPATION** – Job category  
- **TRAVTIME** – Daily commute time (minutes)  
- **CAR_USE** – Primary car use (`Private` / `Commercial`)  
- **BLUEBOOK** – Estimated car value  
- **TIF** – Time in Force (policy duration in years)  
- **CAR_TYPE** – Type of car (SUV, Minivan, etc.)  
- **RED_CAR** – Red car indicator  
- **OLDCLAIM** – Total past claim amount  
- **CLM_FREQ** – Number of past claims  
- **REVOKED** – Whether license was revoked  
- **MVR_PTS** – Motor Vehicle Record points (violations)  
- **CLM_AMT** – Current claim amount  
- **CAR_AGE** – Age of the car  
- **CLAIM_FLAG** – **Target variable** (1 = Claim filed, 0 = No claim)  
- **URBANICITY** – Type of area where the policyholder lives  

---

## Summary of Key Findings
Analysis of 10,000+ policy records revealed:  

1. **Driving History is the Strongest Predictor**  
   - Higher **MVR Points** and past claims → more likely to file a claim.  

2. **Demographics Play a Major Role**  
   - **Occupation:** "Blue Collar" professionals had the highest claim rate.  
   - **Income:** Lower-income brackets more likely to file claims.  
   - **Education:** Claim rates decrease with higher education (PhD holders lowest).  

3. **Vehicle Usage is a Critical Factor**  
   - **Commercial use cars** → much higher claim frequency than private.  
   - **Claim Amount vs Car Value** → weak correlation, suggesting possible claim inflation.  

---

## Methodology
The project followed a structured approach:  

1. **Data Cleaning**  
   - Removed symbols (`$`, `,`) from monetary columns and converted to numeric.  
   - Standardized missing values and data formats.  

2. **Exploratory Data Analysis (EDA)**  
   - **Box Plots** → MVR Points, Income distribution.  
   - **Count Plots** → Car Use (Private vs Commercial).  
   - **Scatter Plots** → Car Value vs Claim Amount.  
   - **Bar Plots** → Occupation, Education vs Claim Rate.  
   - **Heatmap** → Correlation matrix of numerical features.  

3. **Insight Synthesis**  
   - Built a comprehensive **high-risk policyholder profile** combining demographics, vehicle use, and past driving history.  

---

##
Conclusion
This project provides a **data-driven foundation** for:  
- Improving **risk scoring models**  
- Detecting potential **fraudulent claims**  
- Supporting **business decision-making** for underwriting and premium setting  

---
