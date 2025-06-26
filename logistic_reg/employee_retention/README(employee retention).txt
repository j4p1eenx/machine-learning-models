Extracted a dataset HR_comma_sep.csv from kaggle.com which had data regarding the past employees who left the company 
like (their salary , satisfaction level , promotion in last 5 yrs , any work accident , working hours and so on
We calculated the mean of all the factors and plotted a graph to determine the impact of each factor 
The observations were:
      Satisfaction level seems to be relatively low (0.44) in employees leaving the firm vs the retained ones (0.66)
      Average monthly hours were higher in employees leaving the firm (199 vs 207)
      Employees who are given promotion were likely to be retained at firm
      Impact of salary was significantly higher in employee retention
From the data analysis so far we can conclude that we will use following variables as independant variables in our model
      Satisfaction Level
      Average Monthly Hours
      Promotion Last 5 Years
      Salary
Also the salary dataset had textual data ('low','high') using one hot encoding (dummies feature in pandas) we converted the salary
column into numeric data and dropped the original salary column
Then using sklearn we trained the model and the result came out to be an array of [0,1,0,1....] (0-> false(employee will stay) , 1-> true(employee will leave)
The accuracy of model was 77%
                                                                                                 
