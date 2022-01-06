# Admisson_PredictionML
Admission Predication  is an app used to predict the Chance of Admission(%)
# APP link   https://mladmissionprediction.herokuapp.com


### The Followind Model Consist of Data with  Feature Column Serial No.	,GRE Score	,TOEFL Score	,University Rating ,	SOP	,LOR ,	CGPA	,Research	 and Our Target Column Chance of Admit, DATA(500rows*9)

* Data has some Missing values(1% to3%) so see the report - https://github.com/reddysrinath16/Admisson_PredictionML/blob/main/ReportAdmission.html
* We have used mean as we dont want any data to be removed
* We have Used ALL the feature columns Except Serial no which is of no user for our model
* Scaling down the Feature Varible to normalize(used StandardScaler) the data or to bring all the data to the same range
* To see the next report if there has been any affect after using StandardScaler - https://github.com/reddysrinath16/Admisson_PredictionML/blob/main/ReportAdmission2.html
* Also we have checked the feature if there is any multicollinearity
* We have Used Linear , Ridge (also used RidgeCV) , Lasso((also used LassoCV)) and ElasticNet Regression(also used ElasticNetCV)
* The Score is around 84.2512% to 84.195%  and also their adjusted R-Squared(created) but seen that there ans been 2-2.5% decrease in their score
* We Eliminated the ElasticNet as it was least performing one
* ALL the Other 3 Models Score and their adjusted was very slightly same
* The score of all model is slightly the same except Elastic , based on my conclusion i have selected Ridge regression as most of the parameter are contributing towards the dependent variable, we would have select Lasso if the vif factor of some are less than 1 as it literaly penalizes the features(if not useful)



