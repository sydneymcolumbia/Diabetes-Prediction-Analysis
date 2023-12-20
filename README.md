# Diabetes-Prediction-Analysis
Diabetes Prediction Analysis in Pima Indian Female Patients

Overview

This project undertook a comprehensive analysis of the 'diabetes.csv' dataset, sourced from Kaggle's Pima Indians Diabetes Database. The data encompassed variables related to female Pima Indian patients, including the number of pregnancies, plasma glucose concentration, diastolic blood pressure, skin fold thickness, serum insulin level, Body Mass Index (BMI), Diabetes Pedigree Function, age, and diabetes outcome.

Objectives & Methods

The project was methodically structured into several analytical tasks:

Data Loading: The diabetes.csv file was loaded into R for analysis.
Data Splitting: The dataset was divided into training, validation, and test sets with a 40%-30%-30% split, replicating the logic used in the class7.r file.
Classifier Fitting: On the training set, four types of classifiers were fitted using all available predictors: logistic regression, Linear Discriminant Analysis (LDA), Quadratic Discriminant Analysis (QDA), and Naive Bayes.
Sensitivity Analysis and ROC Curves: For a physician-requested target of 85% Sensitivity, ROC curves were plotted for all models. Using the pROC library, the threshold for each model was identified to achieve at least 90% Sensitivity. The best-performing model in terms of Specificity under these conditions was determined.
ROC Curve Comparison: The ROC curves of the logistic regression and LDA classifiers were compared, and any surprises in their performance were discussed.
Winner Model Evaluation: The best model from question 4 was evaluated on the test set using the confusionMatrix function and the computed threshold to check if it met the physicians' Sensitivity requirements.
Specificity Estimate: An estimation was made regarding the Specificity the model would achieve on future patients.
KNN Classifier and Parameter Tuning: A KNN classifier was fitted to the training data, and the parameter 'k' was tuned on the validation set to maximize Sensitivity, adapting code from the class7.r file.
Optimal 'k' Determination: The best value of 'k' was determined based on the tuning process.
KNN Model Evaluation: The KNN model was evaluated on the test set using the confusionMatrix function. Its performance was compared with the winner model of question 4, and a decision was made on which model to recommend to physicians for future diabetes diagnosis in female Pima Indian patients.
Deliverables

The project resulted in a detailed report that provided in-depth analysis and insights into each step. The report not only highlighted the statistical relationships and classifier performances but also offered practical recommendations for medical professionals. The analysis successfully combined data-driven methods with clinical objectives, demonstrating a nuanced approach to predictive modeling in healthcare.
