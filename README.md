# Medical Appointments No-Shows

## Overview
We will be working on the dataset 'No show appoinments' , This dataset collects information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment.
We will be looking at the factors that are important to predict if a patient will show up for their scheduled appointment. Major questions to be answered: 
* Question 1. How does the gap between Scheduled day and Appointment affect the number of patients showing up? 
* Question 2. Does patients receiving an SMS from hospital increases the chance of patients showing up?
* What are the major medical problem patients are suffering from based on gender?, so that hospital can focus on that department more

The original problem description and data set can be found here: https://www.kaggle.com/joniarroba/noshowappointments/home

## Details
I have looked into the dataset and managed a few problems like unifying names, removing wrong data, adding new features based on existing data. I have also investigated most of independent variables in the dataset and made a few observations comparing them to each other as well as to the dependent one (no_show). USed matplotlib and seaborn libraries in developing exploratory data anlaysis. And we came to the conclusion based on these plots. For example, on of the plot generated that answers the third question regarding the disease  based on gender looks as follows:
![111](https://user-images.githubusercontent.com/60280080/83816749-18841700-a691-11ea-99d1-6b7f01d71d9f.png)

For details see analysis documentation Jupyter Notebook

## Conclusion:
The analysis on data tried to solve the question of what factors are important in order to predict if a patient will show up for their scheduled appointment, the factors that are likely to be affecting patients showing up are the following:

* The higher the gap between the scheduled day and the appointment day,higher the chance of patients showing up for their appointments.
* Sending an SMS with a reminder about the appoinment does increase the number of patients showing up by 11% compared to the patients who didn't receive a message.
* It would be great if the hospital can focus on treating Hypertension patients mainly Female wards as many patients suffer from hypertension and something stops them from showing up.
Limitations :
Some of the rows had negative 'Age' as it can't be true, so the data had to be deleted as being an outlier.
Appointment day to visit hospital cannot come before appoinment scheduled day, but many rows had such issues, and had to be deleted. It could have resulted in losing key datas

## Statistical Analysis Scope
- Data Wrangling
- Exploratory Data Analysis (EDA)
- Data visualizations

## Tools
- Python, libraries: numpy, pandas, matplotlib, seaborn, warnings
- Jupyter Lab

