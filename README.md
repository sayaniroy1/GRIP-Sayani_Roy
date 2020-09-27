# GRIP-Sayani_Roy
# Task 2 - To Explore Supervised Machine Learning

In this regression task we will predict the percentage of marks that a student is expected to score based upon the number of hours they studied.
Problem - 
To predict the percentage scores of a student based on his/her hours of study.
What will be predicted score if a student studies for 9.25 hrs in a day?
Data can ve found at - http://bit.ly/w-data

## Importing the libraries
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
%matplotlib inline

## Importing the dataset
url = 'https://raw.githubusercontent.com/AdiPersonalWorks/Random/master/student_scores%20-%20student_scores.csv'
df = pd.read_csv(url, error_bad_lines=False)
print("Data imported successfully")
df.head()

Data imported successfully

Hours	Scores
0	2.5	21
1	5.1	47
2	3.2	27
3	8.5	75
4	3.5	30

## Plotting the distribution of scores
df.plot(x='Hours', y='Scores', style='o')    
plt.xlabel('Hours')  
plt.ylabel('Scores')  
plt.title('Hours vs Scores')
plt.show()

