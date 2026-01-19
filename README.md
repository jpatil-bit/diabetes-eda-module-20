# Predicting 30-Day Hospital Readmission Risk in Diabetic Patients - EDA

## Data Over View
 Data Overview The dataset represents ten years (1999-2008) of clinical care at 130 US hospitals and integrated delivery networks. It includes over 50 features representing patient and hospital outcomes. Information was extracted from the database for encounters that satisfied the following criteria. (1) It is an inpatient encounter (a hospital admission). (2) It is a diabetic encounter, that is, one during which any kind of diabetes was entered into the system as a diagnosis. (3) The length of stay was at least 1 day and at most 14 days. (4) Laboratory tests were performed during the encounter. (5) Medications were administered during the encounter.

The data contains such attributes as patient number, race, gender, age, admission type, time in hospital, medical specialty of admitting physician, number of lab tests performed, HbA1c test result, diagnosis, number of medications, diabetic medications, number of outpatient, inpatient, and emergency visits in the year before the hospitalization, etc.


## Project Overview

The data shows that early hospital readmission among diabetic patients is driven by a combination of age, hospital utilization intensity, medication instability, and admission context. 
While no single variable explains readmission risk, their combined effect creates predictable patterns. Feature engineering revealed that patients with longer stays, more procedures, and frequent medication changes are significantly more likely to be readmitted within 30 days. 
A baseline Logistic Regression model confirmed that these risks can be quantified using ROC-AUC, supporting the idea that early readmission is not random but a measurable outcome that can inform proactive care planning and resource allocation.

---

## Tools and Libraries Used
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For creating static, animated, and interactive visualizations.
- **Seaborn**: For advanced statistical plots and visualization.
- **Jupyter Notebook**: For running and presenting the analysis interactively.
- **colorama** : Exploring this new library for styling and coloring the fonts for the hypothesis.

---

## Dataset
https://github.com/jpatil-bit/diabetes-eda-module-20/blob/main/data/diabetic_data.csv

### Key Features:
* Age
* Gender
* Race
* Time in hospital
* Number of laboratory procedures
* Number of procedures
* Number of medications
* Admission type
* Admission source
* Discharge disposition
* Number of inpatient visits
* Number of emergency visits
* Number of outpatient visits
* Insulin usage
* Diabetes medication indicators
* Medication change count
* Age midpoint (numeric transformation of age ranges)
* Medication change count
* Binary readmission indicator (readmitted within 30 days)

  Excluded Features (to prevent data leakage)

* Patient identifiers (encounter ID, patient number)

* Original readmission category column




---

##  Analysis and hypothesis
*** Jupyter file containes all the EDA's and plots ***

[https://github.com/jpatil-bit/customer-coupon/blob/main/customer_coupon_eda.ipynb](https://github.com/jpatil-bit/diabetes-eda-module-20/blob/main/predict-diabetes.ipynb)

########## **Hypothesize about drivers who accepted the bar coupons** ##########
1. Coupon rejection is more than coupon acceptance. 
2. Coupon acceptance rate is 56.8% , out of which 41.00% is the Bar coupon acceptance. 
3. Drivers over the age of 25 visit bars more frequently (more than once a month) compared to younger age groups.. 
4. Drivers with no kids and not in the occupation of farming, fishing, or forestry visit bars more frequently than parents in others.. 
5. Drivers with age <30 and income <50k , with passanger having no kids , not widowed , visits bar more frequently and visits restaurant < $20 4-8 times a months
   
########## **Hypothesize about drivers who accepted the coffee coupons** ##########
1. Coffee coupon acceptance rate is 49.92%. 
2. Sunny day with temperature of 30 F has more acceptance. 
3. 26 years old singles and 36 years old unmarried partner has more acceptance of coffee coupons. 
4. Male driving to non urgent destination has more acceptance than others. 

---

##  Visualizations

Various visualizations are used in this analysis to uncover insights from the data:

- **Bar Plots**: 

---

##  Getting Started

To run this project locally, follow the steps below:

### Prerequisites

Ensure you have Python 3.x installed and the necessary dependencies:

1. Clone the repository:

   ```bash

   git clone https://github.com/jpatil-bit/diabetes-eda-module-20.git
