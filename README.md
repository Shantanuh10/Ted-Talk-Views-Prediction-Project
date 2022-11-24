# **Ted Talk Views Prediction!** 

![TED-Talks-for-Small-Business-and-Entrepreneurs](https://user-images.githubusercontent.com/87125043/169231039-420bac0a-c5bd-4d28-aafd-ac78717fa3c6.jpg)

# Project Summary

This is a Supervised Machine Learning Regression Project on TED videos dataset.
TED is devoted to spreading powerful ideas on just about any topic. These datasets contain over 4,000 TED talks including transcripts in many languages.
As of 2015, TED and its sister TEDx chapters have published more than 2000 talks for free consumption by the masses and its speaker list boasts of the likes of Al Gore, Jimmy Wales, Shahrukh Khan, and Bill Gates.

The main objective is to build a predictive model, which could help in predicting the views of the videos uploaded on the TEDx website.

As a first step I performed Exploratory Data Analysis (EDA) on the features of the dataset and found correlations between the target variable i.e. ‘views’ column and other columns.

Based on the findings from EDA, I performed Feature Engineering. It is the process of transforming raw data into features that better represent the underlying problem to the predictive models, resulting in improved model accuracy on unseen data.

Next, I did Data Cleaning in which I performed outlier treatment on numerical columns by replacing outliers with extreme values.
After this I performed One-hot encoding using get_dummies function. One-hot encoding turns categorical data into a binary vector representation.
In this dataset, there are only 3 numerical columns out of which 1 is our target variable and 2 can be used as features and rest all columns are either categorical or they contain textual data. So, I generated some numerical columns from these columns.

After this I treated nan values of numerical columns using KNNImputer. KNN Imputer maintains the value and variability of the dataset and it is more precise and efficient than using the average values.

Next, I did Feature selection for numerical features using f_regression.

After this I proceeded to the next step of Fitting the regression models and HyperParameter Tuning.

Lastly, I did the Comparison of different regressor Models for final selection of the Model and found that the best performing regressor model for this dataset is Random Forest Regressor on the basis of MAE with 90% accuracy.



