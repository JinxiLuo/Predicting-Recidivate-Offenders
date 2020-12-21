# Predicting-Recidvate-Offenders

Themes: SAS, Python, Feature Creation, Predicting Recvidisum, Decision Trees, SVM, Random Forest, Neural Network and Ensemble Models

**Project Summary**

This project provides an example of the work layout that I use for my reports, which is avalible for viewing in the two pdfs attached (Part 1 and 2 of Predicting Recidvate Offenders).

The goal for the project was to predict general offender recvidisum using the COMPAS data set for an introductory course in predictive methods. I first apply data cleaning, feature engienerning and selection techinques to try and extract potential usufel features from the dataset. Then a range of Decision Tree, Random Forest, SVM, Neural Network and ensemble models are built and evaluated based on model praremters, feature importance and Balanced Classification Rate with training and validation data. 

**Results**

uouoi

**Structure and Procedures**

 1. Data cleaning, feature enginerring and selection
 
    * New features are created from combinations of categorical varaibles, and dates. AUC and L1 Regression is used from the SciKitlearn Python Libarary to evaluate and choose a smaller subset of features with as high or higher AUC using a decision tree with default parameters to reduce overfitting. 
    
 2. Comparing multiple decision trees in SAS
     
     * Multiple subsets of data set features and decision tree parameters were evaluated to examine the most effective features and parameters to use.
     
 3. Using more complicated models compare predictive accuraries. 
 
     * Random Forest, SVM, Neural Network and Ensemble models are compared using the previous step's data and best decision tree found varying respective major model parameters to determine the best predictive model to use. 


