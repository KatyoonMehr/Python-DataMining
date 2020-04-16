## Python-MedicalCost

#Predicting medical cost of hospitalization based on some factors

#variables:
ID	age	sex	bmi	children	smoker	region	charges	partner
The dataset of insurance contains 10 columns. ID, age, sex, bmi of 1380 patients, whether they have
partner or children, if they are smoker, the region they live, and hospital charges as dependent variable.
Age has 18, smoker 32 and charges 15 missing values.
mean is used to replace age missing values, “unknown” to replace smoker missing values and the 15
rows including missing values of y=charges are dropped. After cleaning we have 1365 rows of data.
Encoding on categorical variables, sex with 2 levels male=1, female=2, , partner with 2 levels yes=1,
no=0, smoker with 3 levels unknown=0, no=1, yes=2 and region with 4 levels northeast=1, northwest=2,
southeast=3 and southwest=4 is done.

#model:
y = -17126.4998 + 221.689 age - 276.906 sex_C + 19300.7 smoker_C - 135.451 region_C - 709.801 partner_C
