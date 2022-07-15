## Telco_Classification_Project
this project will contain information about,
  - project goals 
  - project description 
  - inital hypothesis 
  - Data Dictionary 
  - Steps to reproduce
  - compleate project plan  
  
  ## Goal 
  The Goal of this project is to identify the diffrent attributes causing churn. Mainly focus on our senior ctizens and trying to see the diffrent attributes that are causing ou seniors to chrun  
  
  ## Project desription 
There are sevral reasons as to why our customers are churning here in this project I will explore the diffrent variables that can cause churn esspecilly variables I was not able to look at in previouse project. We will analize the diffrent variables and stick to our main demographic wich is our senior citizens. we will analize the data of our seniors to see diffrnet areas of chun, using data exploration, statistical models and ML classification models and end it off buy reviewing my coonclusions, findings, and recomendations.
 
 ## Initial questions 
 - My First Thoughts
what are the main churn drivers in this data set?
could certaint payment methods be causing the increased ?
how are our senior citizens doing with churn?
what about monthly charges?

## Data Dictionary

#### This is the main data used in Exploration
-------------------------------------------     
- senior_citizen      | non-null  | int64 

- monthly_charges     | non-null  | float64

- tech_support        | non-null  | object 

- payment_type        | non-null  | object
 
- churn               | non-null  | object 

#### This is more data that can be further explored 
---------------------------------------------
- partner             | non-null  | object 
 
- dependents          | non-null  | object 
 
- tenure              | non-null  | int64  

- phone_service       | non-null  | object 

- multiple_lines      | non-null  | object 

- online_security     | non-null  | object 

- online_backup       | non-null  | object 

- device_protection   | non-null  | object 

- streaming_tv         | non-null |  object 

- streaming_movies     | non-null |  object 

- paperless_billing    | non-null |  object 

- total_charges        | non-null  | float64

- contract_type        | non-null  | object 

- internet_service_type  | non-null |  object 

 - gender              | non-null  | object 
 
## Steps to Reproduce

You will need an env.py file that contains your own hostname, username and password of the mySQL database that contains the telco_db
Store that env file locally in the repository.
clone my repo (including the acquire.py and prepare.py) (confirm .gitignore is hiding your env.py file)
libraries used are pandas, matplotlib, seaborn, numpy, sklearn.
you should be able to run final repo.
 
## The Plan

### Wrangle
Modules (acquire.py + prepare.py)

- the acquire.py value will have the code to connedct to the telco database using the main SQL server database for telc_churn as well as a get connecton 
- the prepare.py will have the functions to wangle the data such as
   - dropping null values that where once white pace
   - converting certain collumns to a correct data type 
   - creat dummy variables for certain functions 
   - do a train validate test split on the data 
- Missing values - in the dataset there are no missing values, no further action was taken 
- Doint data split, spilitting data to train validate and test 
  -there is a need to stratify the data so in this case we will stratify by "churn"


### Explore

Here are my Questions I aimed to answer with my exploration and the type of statistical test I did

  - all of these questions do have a visualization 
  
1.Question 1 Are certain payment types indicators of churn?
  - is there a ceratin age group that uses electronic checks ?

2.Question 2 -Are our senior citizen more likely to churn than non seniors ? 


3.Do people who churn have higher monthly charges?
 - how are our senior citizens doing on monthly charges?

4.Question 4 -is someone with tech support more likely to churn?
 -  are seniors mostly using tech support ?
 
 ### Modeling
 My base line prediction is at 73%
In my modeling portion I did three Classification Models
Decision Tree 
Randm Forest 
K-Nearest-Neighbors 
I am going to determing the best one over best accuracy
These models are all evaluated on train, validate and only the best model which is random forest was tested on test data set.

### Conclusion 
- One of the biggest indicators of chrun are our electronic payment method learning from charts the majority of seniors use this type of payment method  
- Overall about half of our senior customers are more likely to churn partly due to the fact that they are paying much more in mothly charges on average than our non seniors

- Our non seniors are much MORE likely to churn due to high monthly charges than our seniors

- We can see that many of our customer who churn, do not use our tech support services, especially our seniors

- the best clasification model turned out to be random forest with the best accuracy 
