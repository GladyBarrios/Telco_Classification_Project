## Telco_Classification_Project
this project will contain information about,
  - project goals 
  - project description 
  - inital hypothesis 
  - Data Dictionary 
  - Steps to reproduce
  - compleate project plan  
  
  ## Goal 
  The Goal of this project is to identify the diffrent attributes causing chun in our company
  
  ## Project desription 
  There are sevral reasons as to why our customers are churning here in this project I will explore the diffrent variables that can cause churn esspecilly variables I was not able to look at in previouse project. We will analize the diffrent variables to find and pin point diffrent reasons for churn, using data exploration, statistical models and ML classification models and end it off buy reviewing my coonclusions and findings. Topt it all off with some recomendations 
 
 ## Initial questions 
 - My First Thoughts
what are the main churn drivers in this data set?
could certaint payment methods be causing the increased ?
how are our senior citizens doing with churn?
what about monthly charges?

## Data Dictionary

- gender              | non-null  | object 
     
- senior_citizen      | non-null  | int64 
 
- partner             | non-null  | object 
 
- dependents          | non-null  | object 
 
- tenure               | non-null | int64  

- phone_service        | non-null | object 

- multiple_lines       | non-null | object 

- online_security      | non-null | object 

- online_backup        | non-null | object 

- device_protection    | non-null | object 

- tech_support         | non-null | object 

- streaming_tv         | non-null |  object 

- streaming_movies     | non-null |  object 

- paperless_billing    | non-null |  object 

- monthly_charges      | non-null  | float64

- total_charges        | non-null  | float64

- churn                | non-null  | object 

- contract_type        | non-null  | object 

- internet_service_type  | non-null |  object 

- payment_type         | non-null  | object
 
 
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
1.

2.

3.

4.

### Modeling
 My base line prediction is at 73%
In my modeling portion I did three Classification Models
Decision Tree 
Randm Forest 
K-Nearest-Neighbors 
I am going to determing the best one over best accuracy
