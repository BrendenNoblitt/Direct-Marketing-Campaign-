# Direct Marketing Campaign: Project Overview 
This project is based off of the Kaggle dataset by Yogesh Patil. This project asks the broad question of explaining AmountSpent in terms of customer characteristics. I chose to focus my analysis on the salary and age of customers, as well as putting a model together to predict the likelihood of a customer with similar characteristics spending over the mean amount spent. 

# Prerequisities 
* SAS Studio 
* SAS 9.4 
* Direct Marketing Dataset: https://www.kaggle.com/yoghurtpatil/direct-marketing

# Exploratory Data Analysis 
After doing some mild data cleaning, I began my exploratory data analysis by looking at the correlation between different numerical variables and the AmountSpent variable. I found that there was a 0.69 correlation between salary and amount spent. I also found that there was a 0.34 correlation between age and AmountSpent. While this is a relatively low correlation, I also found that the middle age variable had a 0.69 associated p value, and therefore, would fail to reject the null hypothesis using this variable, so I took this section of the variable out of my further analysis. I also found that 60% of customers spent below the mean AmountSpent which is $1,217.

# Model Building
After I had concluded that there was a correlation between age and salary with amount spent, I furthered my analysis through a logistic regression model. For the purposes of the model, I created a variable "test_group", and set 0 to customers who spent below the mean amount spent, and 1 for customers who spent above the amount spent. After running the model, setting a variable to predictions, with under 0.5 being "Unlikely" and over 0.5 being "Likely", I ran the frequencies against age and salary. I found that only 36.5% of all customers would be likely to spend over the mean AmountSpent. After further frequency testing, I found that almost 85% of customers would not be willing to spend over the mean amount spent if they had not previously spent over the mean amount spent. I did, however, find that almost 80% of all customers who spent over the mean would be willing to do it again per the predictions created by the model. All other variables had a p value of <0.001, further validating the accuracy of the model. 

# Conclusion 
I found that from the analysis executed, old customers who have previously spent over the mean amount spent were 84% likely to spend over the mean amount spent again. In marketing, this would be a situation where the marketing department could segement and further target the older customers who have already spent over the mean. 
<img src="2.png"
     alt="Markdown Monster icon"
     style="float: left; margin-right: 10px;" />
