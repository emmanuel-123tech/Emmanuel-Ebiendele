# Emmanuel-Ebiendele
Analyze Supermarket Data across the Country - Company XYZ


Company XYZ owns a supermarket chain across the country. Each major branch located in 3 cities across the country recorded sales information for 3 months, to help the company understand sales trends and determine its growth, as the rise of supermarkets competition is seen.


STEP 1-Loading the dataset

The dataset consists of 3 separate csv files of each branch, the 3 files were inserted into a new folder called 'EO' located at my local storage, which have the same csv extension  using os module and glob module.

In other to make the data analysis easier I combined the csv files from each branches known as Abuja_Branch, Lagos_Branch and Port_Harcourt_branch which concatenated into a single csv file called "SUPERMARKET"


After the combination of three dataset into a new single dataset was successful I proceeded by importing the new csv file known as "supermarket" for data exploration.


STEP 2-Data Exploration


In these process i imported the necessary library known as pandas, numpy, seaborn, matplotlib etc.

 After importing the necessary library the next step includes:
(A) Viewing the new dataset with the use of head () function.

 (B) Checking the number of rows using shape attribute which gave me a result of 1000 rows and 17 columns
 
(C) Generating the names of the columns using column attribute 

(D) Making statistical summary of dataset using describe() function to determine the count, mean, standard deviation, minimum, maximum, 25%, 50% and 75% percentile and from my observation : The minimum and Maximum ratio was 4 and 10 respectively while the gross income and Tax statistically looks alike.

 (E) Checking for missing values in the dataset using isnull function from observation there was no missing value in the dataset.
 
 (F) Using the info () function is used to print a concise summary of a Data Frame
 
From the summary above, I  observe that the date and time columns where not in  appropriate data type, in other to make the date and time columns appropriate, i used  the to_datetime() function to convert the date columns to datetime  & Time columns  to datetime then checking the datatype to confirm if they're in datetime format.

STEP 3-Dealing with Datetime Features

The date and Time columns were converted to a Datetime Format which made it easier to extract day, year, month & hour of all activities that occurred in the supermarket sales which was recorded as 11 hours out of 24hours in a day. From the record, it stated the time of occurrence which started from 10am till 8pm using unique () function.

STEP 4-Unique Values in Columns

The nunique () and unique () function methods were used to show the distinct entities and the number of distinct entries in a particular column. 

from observation the following columns shows the number of unique values

(1). Branch- 3 unique values

(2). City- 3 unique values

(3). Customer type- 2 unique values

(4). Gender- 2 unique values

(5). Product Line- 6 unique values

(6). Payment- 3 unique values.

STEP 5- Aggregation with GroupBy

First of all i determined the mean and sum separately using Groupby then combining both the sum and mean into a single table for more understanding.

The Groupby Function made the grouping easier to determine aggregate functions such as sum, mean, minimum and maximum which was performed on the GroupBy object. From my observation

(1).Port Harcourt has the highest total gross income, reason for its highest tax

(2).Lagos has the highest total unit price, quantity and rating

(3).Abuja has the lowest total rating

(4).Port Harcourt paid the highest tax while Lagos paid the least.

(5). Lagos has the highest sum of gross margin percentage, day, month & year while port harcourt has the highest Total & cogs


STEP 6-Data Visualization

In this section i provided answer to some questions by generating charts and making use of different plotting styles such as countplot, catplot & boxplot. I used the Seaborn visualization library to generate various plots. For all visualizations, which include a chart title by using the seaborn set_title method.

Insights

⦁	The minimum and Maximum ratio was 4 and 10 respectively while 

⦁	The gross income and Tax statistically looks alike.

⦁	Port Harcourt has the highest total gross income, reason for its highest tax

⦁	Lagos has the highest total unit price, quantity and rating

⦁	Abuja has the lowest total rating

⦁	Port Harcourt paid the highest tax while Lagos paid the least.

⦁	Lagos has the highest sales record

⦁	Branch (B) Abuja has the lowest total rating

⦁	Epay was the most common Payment used across the 3 branches.

⦁	 Males buy more of Health and beauty

⦁	Females buy more of Fashion accessories & Home and lifestyle than males

⦁	The other three product lines (food and beverages, sports and travel & Electronic accessories) appear equally distributed among the two genders 

⦁	Females spend more on Food and beverages , Fashion accessories & Home and lifestyle than males

⦁	 Males spend more on Health and beauty & sports and travel than females 

⦁	 Both gender spend equally on Electronic accessories

⦁	Electronics has the highest quantity purchased due to its lowest unit price while

⦁	 fashion accessories has the lowest quantity purchased

⦁	Electronics has the lowest unit price while

⦁	 Fashion accessories has the highest unit price

⦁	Epay was mostly used in Lagos, cash was mostly used in port Harcourt and Card was used in Abuja.

STEP 7- Standout Section

In continuation for more insights, i observed that

⦁	Most Customers in Port Harcourt are Females

⦁	The two customer types are equally distributed

⦁	All transactions occurred within 3 months with most sales record in January, followed by march then February

Executive Summary

I ensured to explain each line of code as comment in this notebook


