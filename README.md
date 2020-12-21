# Predicting-Recidivate-Offenders

**Themes**: SAS, Python, Feature Creation, Predicting Recidivism and Multiple Models Comparison.

### Project Summary

This project provides an example of the work layout that I use for my reports, which is available for viewing in the two pdfs attached (Part 1 and 2 of Predicting Recidivism Offenders).

The goal for the project was to predict general offender recidivism using the COMPAS data set for an introductory course in predictive methods. I first apply data cleaning, feature engineering and selection techniques to try and extract potential useful features from the dataset. Then a range of Decision Tree, Random Forest, SVM, Neural Network and ensemble models are built and evaluated based on model parameters, feature importance and Balanced Classification Rate (B.C.R) for an imbalanced class with training and validation data. 

### Results

Derived features from combinations of categorical variables and total previous offense counts were effective at improving model accuracy, however the use of categorical variables resulted in  more complicated trees and did not improve accuracies within models. The COMPAS Decile Score and age were two consistent high importance features, but the results also suggest that Decile score may not be very effective as other available variables such as age and previous offense count had similar high importance.

The final model having highest B.C.R was an ensemble model using majority voting with two of the best predictive models (Decision Tree and Neural Network) obtaining a 69.57% B.C.R improving from the B.C.R of best decision tree model by 0.59%.

### Structure and Procedures

 1. Data cleaning, feature engineering and selection
 
    * New features are created from combinations of categorical variables, and dates. AUC and L1 Regression is used from the Scikit Learn Python Library to evaluate and choose a smaller subset of features with as high or higher AUC using a decision tree with default parameters to reduce overfitting. 
    
 2. Comparing multiple decision trees in SAS
     
     * Multiple subsets of dataset features and decision tree parameters were evaluated to examine the most effective features and parameters to use.
     
 3. Using more complicated models comparing predictive accuracy 
 
     * Random Forest, SVM, Neural Network and Ensemble models are compared using the previous step's data and best decision tree found varying respective major model parameters to determine the best predictive model to use.


