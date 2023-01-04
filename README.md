# Data_Analysis_in_Python
Projects developed as part of the Artificial Intelligence course.


# Folder: Random_Forest - Airline satisfaction DataBase

__Description:__ The dataset describes airline customer satisfaction.

__The dataset includes:__ 
    satisfaction,
	Gender,
	Customer Type,
	Age,
	Type of Travel,
	Class,
	Flight Distance,
	Seat comfort,
	Departure/Arrival time convenient,
	Food and drink,
	Gate location,
	Inflight wifi service,
	Inflight entertainment,
	Online support,
	Ease of Online booking,
	On-board service,
	Leg room service,
	Baggage handling,
	Checkin service,
	Cleanliness,
	Online boarding,
	Departure Delay in Minutes,
	Arrival Delay in Minutes

__Preparing the data to create the model:__ Columns containing string variables were changed to Boolean or numeric variables. In addition, NaN cells were removed and the value 0 entered.

__Creation of decision trees:__ Using all the data in the collection, the level of customer satisfaction with the airline was predicted. The model was checked using the Gini coefficient and Entropy.

The decision tree was then pruned to avoid overtraining. The pruning techniques are pruning maximum depth, leaf size and number of leaf nodes.


The tree model, pruned with constraints, is shown in the graph.

__Creating a random forest:__ a random forest model was created. Evaluations were carried out and the optimal number of trees was found while maintaining efficiency. 

Relevant features for the model were selected. The most important were: Inflight entertainment 0.173599
Seat comfort 0.120732
Ease of online booking 0.091982
Online support 0.058887


# Folder Logistic Regression - Mobile network operator client category

__Context:__
The dataset contains various customer information such as age, region of residence, etc. Contains information downloaded by the telecom company.

__Dataset contains:__
	Description and specificity;
	Region code indicating the area to which customers belong;
	The period for which they have chosen the company;
	Age of the customers;
	Income, average salary;
	Marital status;
	 Address Zone;
	Education group;
	Years of employment;
	Retirement status;
	Gender;
	Code of the area in which they live;
    Customer category.

__Model creation:__ Using the data and the _sklearn.linear_model_ library, a logistic regression model was created and used to assign customers to two, relevant classes. Predictions were then made on the first 10 data set records and 10 random data sets. 

Variables used for prediction in the models:

Model I: income, age

Model II: income, age, gender, employment, paid pension, residence  

__Evaluation of models:__ Each model was evaluated. Accuracy, Precision, Completeness, F1 score were calculated and a confusion matrix was presented.

The data was then divided into a test set and a learning set. A _hold-on_ evaluation was performed and a K-fold cross-validation was carried out. In addition, a ROC curve was plotted. The ROC curve illustrates how high the percentage of misclassifications (positive and negative) will be for a given cut-off point.

Sensitivity/recall ration/sensitivity: the ability of the model to capture positive cases: TP/(TP+FN).
Specificity/Specificity (specificity): ability of the model to capture negative cases: TN/(TN+FP)

Using __ROC__, one can, for example:

-divide the bank's customers into those who will repay the loan and those who will not

-decide what tactics the doctor will take regarding patients

# Folder Dogs 
__Database__ :  Dogs Available for Adoption in the Hungarian Homeless Animals Database (from datahub.io)

__Content:__ 
The data is a compilation of information about dogs that were available for adoption on 12 December 2019 in the Hungarian Homeless Animals Database. There were a total of 2,937 dogs in the database. It contains information about the dogs' names, breed, colour, age, sex, the date they were found and some of their personality traits.

The basic analysis of the database was done.
