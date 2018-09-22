##Assessment

###PLEASE NOTE: I use **PHP** to solve the assessment. Firstly, read the CSV file and get each row/record. Then refactor the row/record with the region is not in an array(“AK and HI”, “48 States”, or “U.S. total”_(I think is "U.S.total" not the "U.S.Total")_), the state is not “District of Columbia” or includes the letter “y”_(Question: should upper case 'Y' be ignroed, too? e.g. Y in 'New York')_. I am not ignroed the case 'Y'. This data will then be used by the following functions to answer all 5 questions.

_________________________

###QUESTION 1 

Which region had the most "Grassland pasture and range" in 1974?

* Answer: Mountain total

###Explanation
Check the year is 1974 in the given data. Then get the larger number of "Grassland pasture and range" to save as the max and save the region as the answer. Compare it with the previous max, if it is greater than previous max, then update max and the answer. 2 regions may have an equal maximum number, if it is, we need to print out both. Return the last answer. It is the answer of Question 1.
__________________________________

###Question 2

How many states had at least 2,000 in the “Land in Urban areas” column for any year prior to 1987?

* Answer: 5


###Explanation

Check the year prior to 1987(< 1987), the “Land in Urban areas” is at least 2000(>= 2000) and the region does not include "total" for each row/record in the given data. If it is true, then save the states as a array. Remove the duplicate values from the array and then count the size of the array. Return the counted number. It will be the number of answer to Question 2.

__________________________________________

###QUESTION 3

What is the average value of the “Cropland used for pasture” column among all states within the Pacific and Mountain regions for 1964?

* Answer: 777.1

###Explanation

Check the states in the Pacific and Mountain regions for 1964 in the given data, sum the value of the “Cropland used for pasture” column in this states and count the size of the value. Then get the average value. This is the answer of Question 3.
________________________________________

###QUESTION 4
Consider the original 13 colonies of England which became what is now the United States. Of the states that have land within the territory of those 13 colonies, which state made the largest contribution to its region's total “Forest-use land” in 2012?

* Answer: Georgia

###Explanation

The 13 colonies were: Delaware, Pennsylvania, New Jersey, Georgia, Connecticut, Massachusetts Bay, Maryland, South Carolina, New Hampshire, Virginia, New York, North Carolina, and Rhode Island and Providence Plantations _[wiki](https://en.wikipedia.org/wiki/Thirteen_Colonies)_. Create a colonies states array of these states. At this array, we should check if these names are written in the same format as in the data file. This is for double verification purposes only and it doesn't have to run every time. _(Question: New York, New Jersey, Pennsylvania contain 'y' or 'Y', should we count them? They are ignored for now.)_

Filter from the given data with the condition that the state is in the colonies states array in 2012. Then find the largest values of the “Forest-use land” and get the state of this value. _(Again, if 2 or more states have the same max value and we need to print out all of them, modify the program.)_ This is the answer of the Question 4.
_______________________________________

###QUESTION 5

Which region has had the largest shift in its land use between 1945 and 2012? Please explain your reasoning, including the data that you used to reach that conclusion.

* Answer: Unknow

###Explanation

For question 5, define 'shift' first, then workout what the answer is under that definition. This question is about reasoning.
 



 
                                    
