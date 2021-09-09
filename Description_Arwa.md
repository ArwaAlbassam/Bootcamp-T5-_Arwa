# **Find the most three stations crowded to set up the centers of the covid-19 vaccine using the MTA Turnstile DataSet**

Arwa AlBassam

**Abstract**


  To reduce the effect and infection of the pandemic in the USA, it should increase the proportion of vaccine recipients. We use the  MTA turnstile dataset to find the three most stations that are more crowded and the three most stations that are more crowded on each of the weekends and weekdays to set up centers for the COVID-19 vaccine.



**Design**

This project originates from the Data Science Bootcamp (T5) to find which stations are more crowded by using the MTA turnstile dataset through exploratory data analysis. 

**Data**

Using the MTA turnstile dataset for the last three months from (http://web.mta.info/developers/turnstile.html). The dataset contains 2932345 rows and 11 features: C/A, UNIT, SCP, STATION, LINE NAME, DIVISION, DATE, TIME, DESc, ENTRIES, and EXIST. The EXIT and ENTRIES columns are integer data types, and the other columns are object datatypes. And we added feature engineering.

**Algorithms**

Feature Engineering:
* DATETIME : Derived DATETIME column from 'DATE' and 'TIME' columns.
* TOTAL_TRAFFIC : Add the TOTAL_ENTRIES and the TOTAL_EXITS columns to find the TOTAL_TRAFFIC.
* Week_Day : To find the name of day using DATE column.
* WEEKEND : To identify if the day is weekend or weekday using Week_Day column.
* TOTAL_TRAFFIC_WEEKDAY : To find the total of traffic on weekday by using the TOTAL_TRAFFIC column.
* TOTAL_TRAFFIC_WEEKEND : To find the total of traffic on weekend by using the TOTAL_TRAFFIC column.

Preprocessing:
* Removing whitespace.
* Check if there are any missing values.
* Remove non-REGULAR values from DESC column.
* Remove the duplicate values.
* Remove the outliers after count the daily entries and daily exits.

Visualization:

Using the Matplotlib and Seaborn to show the Top 3 stations are more crowded and Top 3 stations are more crowded in each of weekday and weekend.

**Tools**

* Numpy and Pandas for data manipulation.
* Matplotlib and Seaborn for plotting.


**Communication**

Presentation.

