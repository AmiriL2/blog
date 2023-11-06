# Data Analytics On The Titanic

## **What's New**
In our previous post, we discussed how to create a To-Do list in Python. Now, we are still using Python, but instead we are using a library called Panda. Panda is an open source library that is used to analyze and manipulate data. With panda, you can open files for the purpose of reading and/or writing over the data.

In addition to using Pandas, we can also use another library called Matplotlib. The purpose of Matplotlib is to graoh data on different kinds of graphs. Examples of these are scatter plots, bargraohs, histograms, pie charts, and more. With the combination of Matplotlib and Pandas, the you can plot specific data from these files on a graph.This could be used for the purpose of making data more readable and easily understandable for people who do not understand programming or higher up managers who only want to see the statistics on this data.

Using these two Python librarys, we will be analyzing data on the passengers from the Titanic.

## **What Is The Titanic?**

The Titanic was part of the one of the most iconic tragedies of all time. RMS Titanic was a British passenger ship that hit an iceberg on its way to New York City from Southampton, England in 1912. While trying to safely escape the titanic, only women and children were allowed to get on the life rafts, while men were told to stay onboard. The others who made it off the ship froze in the fridged water. Of the approximately 2,224 people on board, more than 1500 people lost their lives. The remaining survivors were saved by the RMS Carpathia.

## **The Data**
We were provided with a dataset that contained information on the passengers such as their ID, if they survived, their pclass, name, sex, age, siblings onboard, parch, ticket number, cabin, and embarking status.Here is an example of some of the data that we have:

![Sample of data from Titanic data sheet](/assets/first.png)

## **Question 1**

My first question I developed was to find out what was the morality rate in women onboard the Titanic?

To answer this question I created, i had to find the total amount of females who were onboard the ship and determin using the 'Survived' category if they survived the ship wreck or not. The Survived section used 1s and 0s to tell you if the person survived or not, with 1s meaning survived and 0s meaning they died. This information, I compared the amount of 0s in females to the amount of 1s in females and came out with this graph

![74.2% of females survived the titanic wreck while 25.% of females died](/assets/output.png)

The data presented in the graph reveals that 74.2% of females survived the titanic wreck while 25.% of females died. With this data it can be said that for every 4 females onboard the Titanic, 3 survived and 1 did not.

## **Question 2**

My second question developed was, what percentage of people who payed over $37 survived on the Titanic. This data can be found by finding those who payed more than $37 and finding the percentage of those who survived to those who did not survive. The result was this graph: 

![62% of those who payed over $37 survived while the other 38% did not survive](/assets/output2.png)

The data presented in the graph reveals that 62% of those who payed over $37 survived while the other 38% did not survive. It can be said with this data that more two thirds of those who payed more than $37 survived while the other one third did not. The higher the fare meant the higher up on the Titanic people could be, with the cheaper fares being lower down. This can explain why 2 in 3 people who payed more than $37 survived the events.

## **Question 3**

My third and final question developed from this titanic datasheet is what is the morality rate of those under the age of 18? This can be solved by filterig out all of those who are 18 years or older and checking the survival rate of them in comparison to whose who did not survive. 

![54% of those who were under the age of 18 survived while 46% did not](/assets/output3.png)

This data says that 54% of those who were udner the age of 18 survived while the remaining 46% did not. With this data it can be said that those under the age of 18 had a little more than a 1 in 2 change of surviving. 

## **Conclusion**

In conclusion, the Titanic was a tragic event that resulted in many people losing their lives. 1 in 4 females died on the Titanic, almost 50% of those who were under 18 died, and a little less than 2 in 3 people who payed over $37 for thair fare ended up surviving. If you want to view my full code that created my graphs you can view them here: https://github.com/AmiriL2/Unit2DataScience/blob/main/Titanic.ipynb