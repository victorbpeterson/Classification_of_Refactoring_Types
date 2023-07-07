<h1 align="center">Classification of Refactoring types using Commit messages</h1>

This repository contains code and data for a multi-label classification model for refactoring types based on the commit messages.
The model uses machine learning algorithms to predict the types of refactoring that may be appropriate for a given dataset of commit messages.
Six method-level Refactoring types considered were: Extract Method, Inline Method, Move Method, Pull-up Method, Push-down, Rename.

## Installation
To install the necessary packages, we added a code cell in the beginning of each script with the install commands. No external installation required.

## Usage

The Classification_Of_Refactoring_Types.ipynb script can be used to train and test the model on a given dataset for multi class classification (Phase 2). The FeatureCount.ipynb script can be used to get the useful feaures in the commit messages for each reafactoring type. The Multi-Label_Refactoring_Types.ipynb script can be used to train on different models and predict the refactoring types to get the best performing model.

### Datasets
Datasets used for this project are present in the file Data
- Message.csv is the dataset provided to us for analysis with commit meassges and class ( refactoring types)
- Xtest.csv is the test data with commit meassages after pre-processing for testing the model
- y_pred_gb.csv is the predictions data of gradient boost for feature count in mutli-class classification 
- y_pred_lr.csv is the predictions data of logistic regression for feature count in mutli-class classification 
- y_pred_rf.csv is the predictions data of random forest for feature count in mutli-class classification 
- y_test.csv is the test data with classes for testing the model

### Scripts:
1. Classification_Of_Refactoring_Types.ipynb script has be used to train the model on a given dataset. (phase 2)
The script requires Message.csv dataset
	- #### Model 
		- Random Forest
		- Gradient Boosting
		- Logistic Regression
		- Support Vector Classification
		- Naive Bayes
	- #### Evaluation 
		The model's performance can be evaluated using precision, recall, and F1-score. 
	
2. FeatureCount.ipynb script requires the below datasets (phase 2)
	- Xtest.csv
	- y_pred_gb.csv
	- y_pred_lr.csv
	- y_pred_rf.csv
	- y_test.csv
	
3. Multi-Label_Refactoring_Types.ipynb 
The script requires Message.csv dataset (phase 3)
	- #### Model 
		We have used 3 different approaches namely Label Powerset, Binary Relevance and Classifier Chains.
	
		- Multinomial Naive Bayes
		- Stochastic Gradient Descent
		- Logistic Regression
		- Gaussian Naive Bayes
		- Decision Tree
		- Random Forest
	- #### Evaluation 
		The model's performance can be evaluated using micro and macro average values for precision, recall, and F1-score. Also Subset accuracy and Hamming loss can be used for the multi-label classification.

## Contact
For questions or feedback, please contact the author.
- Victor Peterson (vp4175@g.rit.edu).
- Amulya Reddy Maligireddy (am8735@g.rit.edu), 
- Ashini Anantharaman (aa9162@g.rit.edu), 
- Rahul Gowda Kengeri Kiran (rk1087@g.rit.edu), 

