# Titanic Dataset - Data Cleaning and Exploratory Data Analysis (EDA)
This repository contains an analysis of the Titanic dataset available on Kaggle. The goal of this project was to perform data cleaning and exploratory data analysis (EDA) to identify patterns and trends in the data that may help predict the survival of passengers aboard the Titanic. This was an internship task as part of SkillCraft Technology's Data Science program.

## Dataset Source
The dataset used in this project is from the Kaggle Titanic competition.

## Steps Taken
### Step 1: Load the Titanic Dataset
The Titanic dataset was loaded into a pandas DataFrame for analysis.

### Step 2: Data Cleaning
The following steps were performed to clean the data:

Missing Values: Missing values were handled by imputing the Age column with the median, filling missing Embarked values with the most frequent embarkation point, and dropping the Cabin column due to excessive missing values.
Data Types: Columns like Survived, Pclass, and Embarked were converted to categorical data types to improve analysis.
### Step 3: Exploratory Data Analysis (EDA)
EDA was conducted to understand the relationships between various features and survival rates:

Summary Statistics: A quick overview of numerical features was generated.
Visualizations: Distributions for key features like Age, Fare, and Survived were visualized. We also explored survival rates by Sex, Pclass, Age, and Embarked.
Correlation Analysis: A correlation matrix was created to identify relationships between numerical features.
### Step 4: Feature Engineering
New features were created to better capture information:

FamilySize: Combined the number of siblings/spouses (SibSp) and parents/children (Parch) to create a new feature.
IsAlone: A binary feature indicating whether a passenger was traveling alone (based on the FamilySize feature).
### Step 5: Feature Importance
A Random Forest Classifier was used to assess the importance of different features in predicting survival. The most important features were identified and ranked.

### Step 6: Conclusion
Based on the data analysis, we can draw several conclusions:

Women had a higher survival rate than men.
First-class passengers had a higher survival rate than those in lower classes.
Younger passengers had a higher chance of survival.
Passengers who embarked at Cherbourg (C) had a higher survival rate than those who embarked at Southampton (S) or Queenstown (Q).
