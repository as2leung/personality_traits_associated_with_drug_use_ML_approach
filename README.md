# Personality Trait and Socio-Demographic Risk Factors Associated with Drug & Alcohol Use: A Machine-Learning Approach 

EXAMINING THE SOCIO-DEMOGRAPHIC AND PERSONALITY RISK FACTORS ASSOCIATED WITH DRUG USE: A MACHINE-LEARNING APPROACH



## Table of Contents
* [Purpose of Project](#purpose-of-project)
* [Abstract](#abstract)
* [List of key files](#list_of_key_files)
* [Python Libraries](#python_libraries)
* [Methodology](#methodology)
* [Results](#results)
* [Conclusion](#conclusion)
* [Creator & Credits](#creators)


## Purpose of Project


## Abstract

_**Introduction:**_

Alcohol consumption, illicit drug use and non-illicit drug use represent a major source of mortality and morbidity, as well as social and economic costs in Canada(Canada, 2019; Thomas & Davis, 2007). Studies have highlighted the complex relationship between drug use and a range of factors, including psychological, geographical, environmental, socio-economic, and individual risk factors (Cleveland, Feinberg, Bontempo, & Greenberg, 2008; Ventura, de Souza, Hayashida, & Ferreira, 2015). Improving our understanding of how these risk factors contribute to alcohol and drug use can create more effective individual-level treatments and help health agencies craft policies and programs that provide harm-reduction and enable prevention-based approaches. 

_**Dataset and Research Questions:**_

The current data set includes 1885 respondents and their usage of eighteen different illicit and non-illicit drugs (Dua & Graff, 2019). These eighteen different drugs can be groupd into three major classes of substances: Stimulants, Depressants and Hallucinogens.

 Respondent demographics and five dimensions of personality following the five-factor model (Terracciano, Löckenhoff, Crum, Bienvenu, & Costa, 2008) are also included in the dataset which provide the opportunity to make use of machine-learning approaches to better understand the association between socio-demographic and personality traits with alcohol and drug use. The following research questions can be addressed:

1)	What is the relationship between the risk factors of personality, gender, education, nationality, age, and other attributes on the risk of consumption of each class of drug? Do these relationships change for the various classes of drugs? 

2)	What is the socio-demographic and personality profile of users of the different classes of drugs? Do distinctly different profiles exist?

3)	Can we determine which machine-learning approaches/methods are the most effective for predicting consumption? Do certain algorithms work more effectively for predicting the consumption of different drugs?
In the exploratory analysis and data mining phase of the project, there will be additional opportunities to unearth new questions that we can also answer.

_**Methods & Analysis:**_

To obtain a detailed understanding of the respondents, exploratory analysis will be performed including descriptive statistics, visualizations and data mining. Data quality will be assessed, and data transformations will be identified for data cleaning and feature engineering. Understanding the central tendencies and outliers will also aid in developing profiles for users by drug type and highlight significant usage patterns that can be further explored. K-means or k-median could also be employed to cluster individual attributes to identify unique user profiles.

A preliminary analysis of the data shows that drug use is captured in frequency categories, indicating that a classification approach would be most appropriate in analyzing the data. There is also the potential to group drug use labels into binary outcomes or leave them as multi-class problems. Potential algorithms that I will use and evaluate include:

•	Logistic Regression
•	Multinomial Logit Regression (Softmax Regression)
•	Support Vector Machines
•	Decision Trees/Random Forests/Gradient Boosted Trees
•	K-Nearest Neighbours classifier
•	Linear Discriminant Analysis (LDA)

Finally, to determine the best set of hyperparameters and features, correlation analysis, principal component analysis, GridSerachCV and different metrics will be applied in model evaluation.
 
## File structure and list of key files <a name="list_of_key_files"></a>

* **app folder**
	* template folder
		* *master.html*  # main page of web app - displays three visualizations
		* *go.html*  # classification result page of web app
	* run.py  # Flask file that runs app (change host ip address here)

* **data**
	* *disaster_categories.csv*  # data to process 
	* *disaster_messages.csv*  # data to process
	* *process_data.py*		   #ETL pipeline script		
	* *InsertDatabaseName.db*   # database to save clean data to

* **models**
	* *train_classifier.py* #ML pipeline script
	* *classifier.pkl*  # saved model 

* **README.md**

## Python_Libraries

* nltk
* sklearn
* joblib
* sqlqlchemy
* time
* numpy
* re
* pandas

## Methodology

## Results

The outcome variables for this dataset are all categorical and multiclass, therefore the overall goal will be maximizing the accuracy score of the predictions. However, it will also be important to see trade-offs between precision and recall, so those metrics will be monitored directly as well. The F1 score and the average precision score are also good measures when then are class imbalances, so those will be included as well. Along with recording model scores, I will record the processing time for each model and will fill out a results table like the one in Table 1 below.

<b>Model summary performance metrics </b>
| Metric | Model | Score | Processing Time for Model |
| :--- | :----: | :----: | :----: |
| Accuracy  | | |  |
| Precision/Specificity |  | | | 
| Recall/Sensitivity | | |  |
| AUC |  |  |  | 
| Average Precision Score | | | |


## Conclusion

At the conclusion of the study, I will summarize the findings, discussion, and limitations of the study in this section. It will address the following items:

	1.	What is the relationship between the risk factors of personality, gender, education, nationality, age, and other attributes on the risk of consumption of stimulants, depressants, and hallucinogens?
	2.	How effective were the machine learning models at predicting the risk of consumption of stimulants, depressants, and hallucinogens according to the evaluation metrics?
		a.	What was the best approach?
	3.	How does this study contribute to the existing body of literature?
	4.	What are the limitations of the study and future research avenues?


## Creators & Credits <a name="creators"></a>

* Andrew Leung
    - [https://github.com/as2leung](https://github.com/as2leung)