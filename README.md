# Project_4

## Group Members: 
Brian Lee \
Yu-Hsi (Joy) Chen\
Ilkay Ates\
Roy Jiang\
Alexis Valdez

## Project Description:
This project will utilize healthcare data from stroke patients to gather extensive clinical data. The collected data will be anlyzed and build the machine learning model to understand which features (gender, age, hypertension, and etc) mainly determine stroke potential. The analysis will include the correlation between each features and targeted result (have stroke or not). The project will provide valuable insights for doctors, clinical studies, and the general public health on the effects and prevention of strokes. Pandas, maplotlib, and SQL will be utilized to visualize the stroke predictions. 

## Questions to ask:
1. What Socioeconomic status of people will have a higher chance of strokes?
2. Will analyzing data reveal that strokes are affected by marriage?
3. Do smokers have a higher risk of having a stroke?
4. Is diet affecting likelihood  of having a stroke?
5. What age is it more expected?
6. Which feature in our dataset impact on the possibility of stroke? 

## Parameters to consider:
gender \
age \
hypertension \
heart_disease \
ever_married \
work_type \
Residence_type \
avg_glucose_level \
bmi \
smoking_status \ 


## Resources:
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

### Breakdown of Tasks:
1. Research potential data sources
2. Machine learning: \
  The data is cleaned, normalized, and standardized prior to modeling (from sql or spark) \
  Machine learning model building
3. Data Visualization: \
  Matplotlib \
  Tableau
  
  ### Methods and Results:
We used random forest classifier to first conduct machine learning. We achived good accuracy but very low recall for '1' stroke cases. We then attempted to reduce unbalanced data by using smote() and improved recall by 10%.

Smote:

![Screenshot 2023-04-05 at 9 12 23 PM](https://user-images.githubusercontent.com/114886937/230270326-541a615f-e1d7-4c53-89f7-0ea36b1aaa2b.png)


We further used Logisticregression and SVM with various model tuning and achieved ~10-17% recall.
Logistic regression: 

![logistic-v1](https://user-images.githubusercontent.com/114886937/230269901-65b337e8-a231-40f0-80e1-d306739a3f7d.png) \
![Logistic-v2](https://user-images.githubusercontent.com/114886937/230269907-b6e970c0-0b16-42db-bba0-5ab7dd8d397f.png) \
![logistic-v3](https://user-images.githubusercontent.com/114886937/230269913-622f64f5-b206-47a4-a928-cebb3bb015b6.png) \

SVM:  

![svm-linear](https://user-images.githubusercontent.com/114886937/230269938-71fa305d-d2c9-4c6c-a7ef-a6f6dccd3c99.png) \
![svm-grid](https://user-images.githubusercontent.com/114886937/230269941-50db60a1-89b9-4fd0-8190-11b4802ce302.png) \

Summary: \
![Screenshot 2023-04-05 at 9 11 41 PM](https://user-images.githubusercontent.com/114886937/230270240-a9960f4d-c5dd-4cd2-8503-71891df60aa3.png)

