# BikeShare

## How does a bike-share navigate speedy success
## Author: Zelibe Emeka Samuel
## Date: 20/06/2024.

### ASK:
#### What is the problem you are trying to solve?
The goal of this case study is to convert casual riders to annual members. The case study will identify the behavior of annual
members and casual riders in order to identify and implement a marketing strategy to help convert casual riders into annual members.

#### How can your insights drive business decisions?
The insight can help the marketing strategy by increasing the number of annual members.

#### Business task?
To maximize the number of annual members i will design marketing strategies by finding trends and patterns among casual riders and annual members and identifying casual riders that can be converted to annual members.

#### Key Stakeholders
+ Director of marketing(Lily Moreno)
+ Cylistic executive team
+ Cyclistic marketing analytics team

#### Clear statement of the business task?
The purpose of this project is to identify how annual members use Cyclistic bikes differently from casual riders in order to create a marketing strategy to encourage casual riders become annual members.

### PREPARE
#### Where is the data located?
The public dataset is located https://divvy-tripdata.s3.amazonaws.com/index.html ,the data has been made available by Motivate International Inc. under the license.

#### How is the data organized?
We obtained the Cyclistic historical data trips from July 2023 to June 2024 and organized them in csv format by extracting all the zip files into a folder named “202306-202405_Cyclistic_data”

#### Are there issues with bias or credibility in this data? Does your data ROCCC?
The data being a first party data collected by the company is very credible. This data is ROCCC(Reliable, Original, Comprehensive, Current and Cited).

#### How are you addressing licensing, privacy, security, and accessibility?
The data has been made available by Motivate International Inc. under this license.) This is public data that you can use to explore how different customer types are using Cyclistic bikes. But note that data-privacy issues prohibit you from using riders’ personally identifiable information.

#### How did you verify the data’s integrity?
The data types: 2023 and 2024 are consistent as they possess the same columns and attribute.

#### How does it help you answer your question?
The datasets contain columns such as started_at, ended_at, started_statio, member_casual which can be used to identify bike riders behaviors.The station latitude and longitude columns are helpful for visualization.

#### Are there any problems with the data?
There were some records where the start date was later than the end date.

The datasets was uploaded in my R Project Case 1 document and used the directory to store data.

The data is organized by month from July 2023 - June 2024 and consistent with the month.

The data is sorted and filtered using R.

Installing and loading required packages

#### A description of all data sources used

The data used will be for 12 months and each file contains 13 columns below:
+ ride_id
+ rideable_type
+ started_at
+ ended_at
+ start_station_name
+ start_station_id
+ start_lat
+ start_lng
+ end_lat
+ end_lng
+ member_casual.

### PROCESS
#### What tools are you choosing and why?
Due to the dataset being large, the R programming Language will be used for the cleaning process and analysis.

#### Have you ensured your data’s integrity?
The dataset is complete as it contains the required component,the data is consistent,credible and trustworthy.

#### What steps have you taken to ensure that your data is clean?
I removed duplicates, i removed NA’s then i removed empty rows and column,checked the unique value in each variable for misspellings using count().

#### How can you verify that your data is clean and ready to analyze?
I checked for missing values using the filter() function, i checked the variable unique values using the count() function and i checked for duplicates using the duplicated() function.


### ANALYZE

#### Summary of the Analysis
The recent 12 months’ trip data shows that membership riders’ riding numbers are higher than casual riders. Meanwhile, the casual rider’s usage time is longer than the membership riders.The data shows that casual riders use the service more at the weekend.

### SHARE
After analyzing the data and having an insight on how casual riders and membership riders use cyclistic bikes differently i used R (ggplot2) to make the visualization. Some of the key findings were:

1. The membership and casual riders proportions were 69% and 31% respectively
2. Total bike usage has significantly changed seeing a peak in July,August and October and seeing a significant drop in Dec and Jan 2024.
3. The average trip duration shows that casual riders ride longer than membership riders especially on weekends.
4. The weekday usage shows that more membership riders mainly use the weekdays and casual riders use the weekends especially on Saturdays.
5. Electronic bikes, docked bikes and classic bikes are used by casual riders while membership riders use only electronic bikes and classic bikes.

### ACT
Following the analysis of the difference between casual riders and membership riders,we can devise marketing strategies to encourage casual riders to convert to members. The following recommendations are suggested:

1. Since casual riders tend to ride longer than members,providing discounts for extended ride durations could serve as an incentive for casual riders and also encourage members to ride for longer periods.
2. We can increase the rental prices for the weekends and then provide discounts and offers to casual riders if they convert to members for weekends and summers.
3. Priority availability access can be introduced for members during the weekends and summers.
