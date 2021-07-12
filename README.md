# ETL_Nord_Spar_ATM_Transactions

The task was to build a batch ETL pipeline to read transactional data from RDS, transform it using PySpark and then load it into Amazon S3 ---> RedShift Tables

Banks have to refill the ATMs when the money goes below a specific threshold limit. 
This depends on the activity and the area where a particular ATM is located as well as the weather, day of the week, etc.
In our project, we try to observe the withdrawal behaviour and the corresponding dependent factors to optimally manage the refill frequency. 
Apart from this, other insights also have to be drawn from the data.

 
Analysing the data to find :
Top 10 ATMs where most transactions are in the ’inactive’ state
Number of ATM failures corresponding to the different weather conditions recorded at the time of the transactions
Top 10 ATMs with the most number of transactions throughout the year
Number of overall ATM transactions going inactive per month for each month
Top 10 ATMs with the highest total amount withdrawn throughout the year
Number of failed ATM transactions across various card types
Top 10 records with the number of transactions ordered by the ATM_number, ATM_manufacturer, location, weekend_flag and then total_transaction_count, on weekdays and on weekends throughout the year
 

We have data from more than 100 ATMs across Denmark. Data is captured for every transaction including, card type, location, date, time, ATM type, etc.
Dataset from https://www.kaggle.com/sparnord/danish-atm-transactions

Note : The transaction amount field in the data set was added separately using a random function for the analysis purpose. 

 
