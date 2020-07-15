# Project 4: Hackathon

### Contents:
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Data Sources](#Data-Sources)
- [Data Dictionary](#Data-Dictionary)
- [Conclusions/Recommendations](#Conclusions)

<a id=Problem Statement></a>
## Problem Statement

Given a dataset of features with education, income, and lifestyle related data find the best model and combination of features, with a twenty (20) feature maximum, to predict if a person's income is <=50K or >50K.

<a id=Executive Summary></a>
## Executive Summary
The team used a large dataset with 32,561 rows and 14 columns to train a prediction model. In total 6 classification models were run several times. In each round the number of features and hyperparameters were changed. Out of 3 rounds of 6 models, the best accuracy scores in the training and testing datasets are from random forest classifier model. Random forest classifier with the optimum hyperparameters returned 84% accuracy on the testing dataset. The team has to be very conscientious about the number of features and hyperparameters because of the constraint that was stated in the problem statement. The best performing model used 13 features.

<a id=Data Sources></a>
## Data Sources
[large_train_sample](data/large_train_sample.csv) <br>
[cheap_train_sample](data/cheap_train_sample.csv) <br>
[test_data](data/test_data.csv) <br>

<a id=Data Dictionary></a>
## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**age**|*int*|large_train_sample|continuous|
|**workclass**|*object*|large_train_sample|Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.|
|**fnlwgt**|*int*|large_train_sample|continuous|
|**education**|*object*|large_train_sample|Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.|
|**education_num**|*int*|large_train_sample|continuous|
|**marital_status**|*object*|large_train_sample|Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse|
|**occupation**|*object*|large_train_sample|Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces|
|**relationship**|*object*|large_train_sample|Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried|
|**sex**|*object*|large_train_sample|Female, Male|
|**capital_gain**|*int*|large_train_sample|continuous|
|**capital_loss**|*int*|large_train_sample|continuous|
|**hours_per_week**|*int*|large_train_sample|continuous|
|**native_country**|*object*|large_train_sample|United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands|
|**wage**|*object*|large_train_sample|>50K, <=50K|

<a id=Conclusions></a>
## Conclusions

Random Forest was the best performing model with a combination of only thirteen (13) features. The final Training Accuracy Score was 84.5% and the final Testing Accuracy Score was 84.6%.  Eight (8) of the features were engineered with six (6) features created from 'marial_status' and two (2) features engineered from 'workclass.' The remaining features came directly from the raw dataset. Two other models , Logistic Regression and Support Vector Classifier, scored similarly but had slightly lower scores and a Training Accuracy Score that was slightly greater than the Testing Accuracy Score. 










