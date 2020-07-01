# Heart-Disease-Classification-Project
> Heart Disease Classification using UCI Heart Disease Dataset.



# Data Analysis of the Heart-Diseases-Project

## 1) Defining the problem statement.
### Predict whether a patient has a heart disease or not based on certain attributes.

## 2) Data
The original data came from the Cleavland data from the UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/heart+Disease

There is also a version of it available on Kaggle. https://www.kaggle.com/ronitf/heart-disease-uci

## 3) Decide on Evaluation Metrics
### Decide what defines success?
* Achieving a certain amount of accuracy
* Limiting the number of false negatives or false positives

> Since, We have to do medical predictions they need to be very accurate and there must be very 
> less false negatives to prevent disease going undetected.
> Here we aim for around 95% accuracy.
## 4. Features

This is where you'll get different information about each of the features in your data. 
You can do this via doing your own research (such as looking at the links above) or 
by talking to a subject matter expert (someone who knows about the dataset).


## Data Dictionary

**Create data dictionary**

1. age - age in years
2. sex - (1 = male; 0 = female)
3. cp - chest pain type
    * 0: Typical angina: chest pain related decrease blood supply to the heart
    * 1: Atypical angina: chest pain not related to heart
    * 2: Non-anginal pain: typically esophageal spasms (non heart related)
    * 3: Asymptomatic: chest pain not showing signs of disease
4. trestbps - resting blood pressure (in mm Hg on admission to the hospital) anything above 130-140 is typically cause for concern
5. chol - serum cholestoral in mg/dl
    * serum = LDL + HDL + .2 * triglycerides
    * above 200 is cause for concern
6. fbs - (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
    * '>126' mg/dL signals diabetes
7. restecg - resting electrocardiographic results
    * 0: Nothing to note
    * 1: ST-T Wave abnormality
        * can range from mild symptoms to severe problems
        * signals non-normal heart beat
    * 2: Possible or definite left ventricular hypertrophy
        * Enlarged heart's main pumping chamber
8. thalach - maximum heart rate achieved
9. exang - exercise induced angina (1 = yes; 0 = no)
10. oldpeak - ST depression induced by exercise relative to rest looks at stress of heart during excercise unhealthy heart will stress more
11. slope - the slope of the peak exercise ST segment
    * 0: Upsloping: better heart rate with excercise (uncommon)
    * 1: Flatsloping: minimal change (typical healthy heart)
    * 2: Downslopins: signs of unhealthy heart
12. ca - number of major vessels (0-3) colored by flourosopy
    * colored vessel means the doctor can see the blood passing through
    * the more blood movement the better (no clots)
13. thal - thalium stress result
    * 1,3: normal
    * 6: fixed defect: used to be defect but ok now
    * 7: reversable defect: no proper blood movement when excercising
14. target - have disease or not (1=yes, 0=no) (= the predicted attribute)


## Data Analysis involves

* Obtain data and see if it is in a format that can be used for predictions
* Check for missing values
* Find patterns in the data
* Check whether the features associated with the data make sense
* Convert non numeric or object values to numbers so that they can be fed to ML models
* Becoming a subject matter expert

> include above points
## Data Exploration (exploratory data analysis or EDA)

The goal here is to find out more about the data and become a subject matter export on the dataset you're working with. 

1. What question(s) are you trying to solve?
2. What kind of data do we have and how do we treat different types?
3. What's missing from the data and how do you deal with it?
4. Where are the outliers and why should you care about them?
5. How can you add, change or remove features to get more out of your data?



# Modelling and Experimentation
### Select models according to the problem statement. Here we have Classification problem so the models best for CLassification are used.
> For more information on models for specific problems visit: https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html

### Here we use:
* K Nearest Neighbours Classifier
* Logistic Regression
* Random Forest CLassifier

### After fiting each of these on the default parameters we get a baseline model and then we work on Experimentation and Evaluation.
### Experimentation and Evaluation involves:
* Hyperparameter tuning
* Feature importance
* Confusion matrix
* Cross-validation
* Precision
* Recall
* F1 score
* Classification report
* ROC curve
* Area under the curve (AUC)

