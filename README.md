# British-Airways-Data-Science --  Forage
Two-part British Airways Data Science Virtual Experience covering lounge eligibility modelling and customer booking prediction using Python, data analysis, and Random Forest.



## 📌 Project Overview

This repository contains both parts of the virtual experience:

### Part 1 — Modelling Lounge Eligibility

Developed a reusable **lounge eligibility lookup model** for British Airways' Heathrow Terminal 3 operations.

The model groups flights using three stable operational dimensions:

* **Route type:** Short-haul vs. Long-haul
* **Destination region:** Europe/UK, North America, Asia/Pacific, Middle East/Africa, and Latin America/Caribbean
* **Departure time:** Early morning, Mid-day, and Evening

The lookup table estimates the proportion of passengers falling into different lounge eligibility tiers. The approach is designed to be reusable for future flight schedules without relying on specific flight numbers, aircraft types, or dates.

The project also documents the assumptions behind passenger eligibility and demonstrates how the lookup structure can be incorporated into future scheduling and capacity-planning analysis.

### Part 2 — Predicting Customer Booking Behaviour

Built a **Random Forest classification model** to predict which customers are most likely to complete a flight booking after making a search.

The dataset contains **50,000 flight-booking searches and 14 original features**, with a booking conversion rate of approximately **14.96%**.

The analysis included:

* Exploratory data analysis
* Feature engineering
* Handling high-cardinality categorical variables through frequency encoding
* Creation of behavioural and route-level features
* Stratified train/test splitting
* 5-fold cross-validation
* Random Forest model training
* Class-imbalance handling
* Feature importance analysis
* ROC-AUC, precision, and recall evaluation

The final Random Forest model used **500 trees**, a maximum depth of **12**, and balanced class weights.

### 📈 Key Results

The model achieved:

* **ROC-AUC:** 0.79
* **Recall:** 68%
* **Precision:** 32%
* **Cross-validation ROC-AUC:** 0.78

The model was deliberately optimized toward **higher recall**, allowing the business to identify a larger proportion of potential bookers for targeted marketing and operational decision-making.

Feature importance analysis identified **booking origin** as the strongest predictor, followed by route and airport popularity.

## 🛠️ Skills & Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Exploratory Data Analysis
* Feature Engineering
* Classification
* Random Forest
* Cross-Validation
* Model Evaluation
* Data Visualisation
* Business Analytics
* Predictive Modelling
* Data-driven Decision Making

## 🎯 Business Impact

Together, the two projects demonstrate how data science can support different areas of airline operations — from **estimating lounge demand and passenger eligibility** to **identifying customers with a high likelihood of completing a booking**.

The booking prediction model can support prioritisation of high-propensity customers, targeted promotional campaigns, and operational planning.

This project strengthened my ability to translate a business problem into a structured analytical solution and communicate technical findings in a way that supports practical business decisions.
