##Assessment

###PLEASE NOTE: I use **PHP** to solve the assessment. Firstly, read the CSV file and get each row/record. Then refactor the row/record with '0' in the zip where the school is not Proprietary or Foreign. This data list will then be used by the following functions to answer all 5 questions.

###Take a function to convert string to integers or floats as necessary. Replaces ('$-' or '-') with 0. 
_________________________

###QUESTION 1 

Please provide your answer as a number. How many schools had disbursed a total of greater than or equal to $707,300 and less than $800,895 in loans for the time period reported on the spreadsheet provided (“Quarterly Activity” only)?

* Answer: 58

###Explanation
Create a function to sum all disbursements for each row/record in the given data and check the sum value if it is in a defined range (i.e., >= 707,300 and < 800895). If it is true, then count it. Return the counted number.It will be the number of schools with total disbursements within the designated range. Call the function to answer Question 1.
__________________________________

###Question 2


Consider the sum of expected total loan amount if the loans were fully disbursed for each school in this Quarter. For how many schools was this amount greater than $20,000,000?

* Answer: 75


###Explanation

Take a function to sum all amounts of loans originated for each row/record in the given data and check the sum value if it is greater than the minimun specified (i.e., > 20,000,000). If it is true, then count it. Return the counted number. It will be the number of schools with total expected loan amounts greater than the minimum. Call the function to answer Question 2.
__________________________________________

###QUESTION 3

Amongst the schools that are considered part of Bellevue, WA (according to zip codes on http://zipcode.org), what was the largest number of recipients within a school for either DL Unsubsidized Undergraduate or DL Unsubsidized Graduate loans? Ignore unavailable data i.e. data with ‘-’ value.

* Answer: 219

###Explanation

Take a function to check the zipcode of school in the given data with the zip code in the array of Bellevue zip codes. If it is in the array of Bellevue zip codes, get the greater number of recipients when comparing DL Unsubsidized Undergraduate and DL Unsubsidized Graduate to save as the max. Compare it with the previous max, if it is greater than previous max, then update max. Return the last maximun number. Call the function to answer Question 3.

________________________________________

###QUESTION 4
Consider the state in which the last Olympics was hosted in the USA. What is the sum of the expected total loan amount if the loan is fully disbursed for DL Subsidized loans in the public schools in this state in Q4 of 2016-2017, based on the data provided?

* Answer: $7,912,715.00

###Explanation

The state in which the last Olympics was hosted is UT. Take a function to find the record that it is in the UT and #of school type Public, the $ of Loans Originated for DLSubsidized loans in the given data. Then sum the amount of loans originated in the new records. Return the number. Call the function. That will be the sum of expected total loan amount if the loan is fully disbursed for DL Subsidized Loans in Public schools in Utah. 

_______________________________________

###QUESTION 5

Consider all the private nonprofit schools in WA state where the name of the school starts with either “s”, “u”, “v” or “w”. For these schools, consider the expected total loan amount if the loan is fully disbursed for unsubsidized undergraduate studies. Exclude all schools where the unsubsidized undergraduate loan amount is not available i.e. “-” or 0. What was the median value?

* Answer: $79,524

###Explanation

Create a first letters array. Filter from the given data with the condition that the type of loan is "DL Unsubsidized Undergraduate", the state equals "WA", the schools is "Private-Nonprofit", and the first letter of the school's name is in the first letters array. Save the amount of loans originated as a new array and then use the calculate median value function searched from google to return the median value. Call the function to answer Question 5.