# CYCLISTIC Bikeshare user engagement Analysis

## Table of Content 
1. [Overview](#Ove#rview)
2. [Data Source](##Data-Source)
3. [Tools](##Tools)
4. [Skills demonstrated](##Skills-demonstrated)
5. [Stored procedures](##Stored-procedures-in-R)
6. [Business questions](##Business-questions)
7. [Recommendation from findings](##Recommendation-from-findings)
8. [Data Visualization  Dashboard](##Data Visualization-Dashboard)

## Overview
This is the portfolio Project for my Coursera Data Analytics certification and in this project I worked on the datasets provided to 
reveal how annual members and casual riders use Cyclistic bikes differently alongside discovering factors that can make casual riders
subscribe to being a full member.

## Data Source
The datasets used for the analysis can be downloaded [here](https://divvy-tripdata.s3.amazonaws.com/index.html)

## Tools 
-	Microsoft Excel - Data Cleaning, Visualization
-	R studio - Data Analysis, Data Transformation

## Skills demonstrated
- Data Cleaning
- Data Analysis
- Data Transformation
- Data Visualization
- Stored Procedures in R

## Stored Procedures in R
```R
August <- read.csv("C:\\Users\\HP\\Downloads\\my coursera portfolio\\202008-divvy-tripdata.csv")
View(August%>%)
Modified_August <- August %>%
select(started_at, ended_at,member_casual) %>%
separate(ended_at, c("end_date", "end_time"), " ") %>%
separate(started_at, c("start_date", "start_time")," ") 
View(Modified_August)
Modified_August$day_of_week <- strftime((Modified_August$start_date), "%A")
 ```

## Business Questions
- How do annual members and casual riders use Cyclistic bikes differently?
- Why would casual riders buy Cyclistic annual memberships? 
- How can Cyclistic use digital media to influence casual riders to become members

## Recommendation from findings
The dataset reveals that the 7th weekday stays on top of the chart for three consecutive years with
a very high ride length, this will be a very good point to generate more revenue by Cyclistic if
they were encourage to subscribe to full membership.
The analysis show that in numbers, the count of those that subscribed to paid mentorship are more
than the casual users but when the ride length of each user is being reviewed over the years, the
casual users have the highest length of usage hours of the bikes from cyclistic and this reveals
that investing enough resources into winning them over to becoming paid members wont be a waste.


## Data Visualization Dashboard
 


