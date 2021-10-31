"# group-project-group-69" 

Files contains:
- Group Project 69 Note Book Final Version.ipynb
    The Final Version of the Note Book   
- Untitled Folder/Bus Card Type.xlsx - Bus Card Type.csv.csv
    Data set after some basic clean
- Untitled Folder/BusCardType.csv
    Orgional data set downloan from Open Data NSW transport at 13 September 2020
- README.md









Project Proposal 

COVID-19 and its Impact on our Public Transportation System
The worldwide pandemic COVID-19 has had major impacts on every aspect of our lives over the past two years. With a large number of countries facing lockdowns to reduce the spread of the virus, people are being forced to minimise their travel and work from home. This has drastically changed the data surrounding public transport in Australia, particularly in regards to the number of passengers using public transport. Looking at this change in data can provide insight into the impact of COVID-19 on the public transport system in Australia.

Project Goal:
We are going to use the bus opal data from Transport NSW to predict the number of passengers for each month if COVID-19 didn’t happen. We will also compare this data with the actual passenger data from during the COVID-19 period. 
-	To predict what would happen with bus trip data if there is no COVID-19. This data will be predicted from March 2020, the approximate start of the COVID-19 impact in Australia.

Data Source and Background:
The dataset we will be using comes from the Transport for NSW website, which has several different types of data available about its services. We will be using the Monthly Opal Bus Trips by Contract Area data, which contains information about opal card usage within the bus system throughout Sydney. 

The data separates opal usage into 17 different categories, based on the type of passenger (such as “Adult”, “Child/Youth”, and “Concession”). This data is categorised on a monthly basis, ranging from July 2016 to August 2021. 

Format:
The original data is in CSV format which has a size of 186,804 bytes. It contains 605 rows and 64 columns in its original version. After the modification of the data file, the data file contains 63 rows and 12 columns in total.

What work needs to be done:
Data Cleaning
Reformate the data: As we only focus on the Sydney Metro Bus Contract 1 from the data set, only the passenger number of contract one is used in the data file. In addition, in order to make the graph plotting process more convenient, the format of the data is changed by transposing the column titles and the row titles, as well as all their matching data’s positions.
Single trip:  Adult and child’s single trip records are also removed from the data file. Both Adult and child’s single trip records have 3 categories, so 6 categories in total.  We have little information about what they represent after going through the Transport NSW website. In addition, the number of passengers in all 6 categories is relatively small, therefore we deleted all six categories of a single trip, and completely removed the single trip child and adult from the data file.
Missing Values: There are several missing values across the dataset, where there were 0 passengers of a certain type for that month. This is more prevalent for the more specific types of passengers, such as “Employees” or “Day Pass Child/Youth w/o SAF”, where it is quite rare to see any sort of value for that month. With these values, we will need to fill the missing slot by inputting a 0 value in each area that is missing values. 
	
Data Manipulation
Predict data: Separate the data frame into two parts, first part is the actual data which include the monthly trip from July 2016 to March 2020.  The second part is the actual data from April 2020 to August 2021. We will use the first part of the actual to predict the second part of the data.
Comparison: To predict the number of passengers if there’s no covid-19,  and compare the data with the actual passenger number during the COVID-19 period. 

Techniques expected to use in the project:
We expect to use predictive modelling techniques such as linear regression to predict the number of passengers in 2020 and 2021, assuming that covid-19 does not exist. The model will be established for each type of passenger, using the number of passengers each month from Jul-16 to Mar-20, since Sydney’s first lockdown started in March 2020, which might strongly influence the number of passengers in the NSW bus system. 

Under the method of linear regression, we will understand the correlation of the data by calculating the correlation coefficient, the mean-squared-error (MSE), and the value of r2.

We will also use several methods of visualisation such as Seaborn and Matplotlib to create graphs to represent the data.

Project Plan:
Week 9 Complete Data Cleaning and Manipulation
Week 11 Run tests and create graphs on data
Week 12 Evaluate data and make comparisons
Week 12 Record Video Presentation

Group Member:
Joshua Johnston - 45934568
Ming Lin - 45958734
Mingxin Yang - 47088877
Ryan Parnell - 47088079
