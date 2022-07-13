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

|    Variable   |    Meaning       |
| ------------- | -------------    |
| gender        | non-null   int64 |
| Content Cell  | Content Cell     |


gender                                 7032 non-null   object 
 5   senior_citizen                         7032 non-null   int64  
 6   partner                                7032 non-null   object 
 7   dependents                             7032 non-null   object 
 8   tenure                                 7032 non-null   int64  
 9   phone_service                          7032 non-null   object 
 10  multiple_lines                         7032 non-null   object 
 11  online_security                        7032 non-null   object 
 12  online_backup                          7032 non-null   object 
 13  device_protection                      7032 non-null   object 
 14  tech_support                           7032 non-null   object 
 15  streaming_tv                           7032 non-null   object 
 16  streaming_movies                       7032 non-null   object 
 17  paperless_billing                      7032 non-null   object 
 18  monthly_charges                        7032 non-null   float64
 19  total_charges                          7032 non-null   float64
 20  churn                                  7032 non-null   object 
 21  contract_type                          7032 non-null   object 
 22  internet_service_type                  7032 non-null   object 
 23  payment_type  
 
 
## Steps to Reproduce

You will need an env.py file that contains your own hostname, username and password of the mySQL database that contains the telco_db
Store that env file locally in the repository.
clone my repo (including the acquire.py and prepare.py) (confirm .gitignore is hiding your env.py file)
libraries used are pandas, matplotlib, seaborn, numpy, sklearn.
you should be able to run final repo.
 
## The Plan

Wrangle
Modules (acquire.py + prepare.py)

- the acquire.py value will have the code to connedct to the telco database using the main SQL server database for telc_churn as well as a get connecton 
- the prepare.py will have the functions to wangle the data such as
   - dropping null values that where once white pace
   - converting certain collumns to a correct data type 
   - creat dummy variables for certain functions 
   - do a train validate test split on the data 
Missing values - in the dataset there are no missing values 

Explore
