# Investigating a Hospital Check up Appoinment Dataset
Data Analytic projects to explore, clean and effectively communicate data showing patients medical appointment history.

## Table of Contents
1.Introduction

2.Data Wrangling

3.Conclusions

## Introduction
Dataset Description
In this project, I set out to analyse a dataset apprising information about 100k medical appointments in Brazil, with the specific focus of showing whether or not patients show up for their appointments. 
The column names in the dataset being analysed are as follows:
ScheduledDay, Neighbourhood, Scholarship, Age, AppointmentDay, Gender, PatientId, AppointmentId, No-show, Hipertension, Diabetes, Alcoholism, Handcap and SMS_received. 
These are the significance of some of the various columns listed.

ScheduledDay: This column provides information on the day the patient scheduled an appointment.

Neighborhood: This column provides information about the location of the hospital for medical checkup.

Scholarship: This column indicates whether a patient is on welfare care program.

Age:This column provides information on the age of the patients.

Gender: This column provides information on whether the patient is a male or female.

AppointmentDay:This column provides information on the actual day for medical checkup/apppointment.

No-show: This column indicates whether or not a patient showed up for an appointment. A No answer indicates a patient showed for the appointment and a Yes answer indicates the patient didn't show up for the appointment.

Hipertension, Diabetes, Alcoholism and Handcap indicates the disease the patient was diadnosed for.

## Question(s) for Analysis
To analyse and effectively communicate information on this dataset, I essentially explored three questions as the basis for my analysis.

1.Is the accessibility to welfare program (scholarships) a major factor in assessing whether patients would show up for their medical appointments or not?

2.Is Age a major factor in determining whether patients would show or not?

3.Does gender play a significant role in determining whether patients would show up for medical appointments or not.

## Data Wrangling
In this section of my report, dataset for my analysis is initially loaded, explored, inspected and described. I check for the tidiness of the dataset, and if neccessary clean/trim the dataset for proper analysis. Also in this section, columns that are not useful for analysis are also eliminated.

## Data Cleaning
In this subsection, I tidy the dataset to get rid of columns that are not useful in my analysis. I also make changes to types of data in the various columns.

The following data assessments were made on the dataset to improve the quality of the dataset for analysis.

1.Column AppointmentID, Patient ID etc. would be dropped since it is not useful in my analysis

2.Datatype in No-show was changed from yes or No to boolean.

3.No-showed column was renamed to Showed-Up

4.Data in age column was checked for invalid data.

5.There are no missing values available in the dataset so no fill in is needed.

6.There are dublicates to be cleaned.


## Drawing Conclusions

### Research Question 1 Is the accessibility to welfare program (scholarships) a major factor in assessing whether patients would show up for their medical appointments or not?

            Showed-up  
Scholarship             
0             0.592860  
1             0.601494  
The mean value of those with scholarship who showed up is almost equal to the mean value of those who showed for appointments without any scholarship.

Therfore, The accessibility to the welfare program cannot be a major determiner in assessing whether patients would show up for their medical appointments. This analysis is further visualized below:

### Research Question 2 Is Age a major factor in determining whether patients would show or not?

average_age
Showed-up
0    48.087105
1    49.352337

It can also be seen that the averages ages of patients who showed up for appointments and those who did not are very close. This information is further visualized below.


### Research Question 3 . Does gender play a significant role in determining whether patients would show up for medical appointments or not?

Gender  Showed-up
F       1            957
        0            686
M       1            838
        0            535

It can be seen that more females showed up and also did not show up for their appointment than males.


gender_showup
Gender
F    0.582471
M    0.610342


From the above analysis, the gender of patients does not play a significant role in determining whether patients would show up for medical appointments. The mean number of females and males who show up for appointments are almost equal.


## Conclusions
The following are summaries of my findings and results based on the research questions I posed initially. Recommendation for additional research is suggested to augment the data set analysis further.

1.The availability or non-availability of scholarship opportunities does not have an effect on whether patients would show up for their appointments.

2.The age of a patient is not a major factor in determining whether a patient would show up for an appointment or not.

3.Also the gender of a patient cannot be a major determiner to assess whether or not a patient will show up for his or her appointment or not.

4.A higher number of females patronized the hospital more than males.

## Limitations
1.My data exploration is limited and based on a limited number of factors around Age, Gender and Scholarship availability.
 Further extensive exploration can be done to explore questions revolving around Appointmentsday, ScheduledDay and neighboorhood
 and how they affect or have an influence on the tendency for patients to show up for their medical apointments.

2.Further discussions can also be done on the column of diseases to further explore how they relate columns such as gender.

## References
1.https://matplotlib.org/stable/index.html

2.https://pandas.pydata.org/docs/

3.https://www.kaggle.com/code/mostafarefaatm/medical-appointment-no-show

4.https://www.kaggle.com/datasets/joniarroba/noshowappointments/code
