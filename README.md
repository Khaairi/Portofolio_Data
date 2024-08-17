# Portofolio
# Cyclistic Case Study
## Introduction
This project is the final assignment for the Google Data Analytics course on Coursera. In the scenario, we act as a junior data analyst working to answer business questions related to maximizing the number of memberships for Cyclistic. Cyclistic is a fictional company that provides bike rental services, with two types of users: membership users and casual users. The Cyclistic marketing team believes that the key to the company's success is maximizing the number of membership users. As analysts, we will conduct the analysis process starting with ask, which involves identifying the business task and creating a list of problems to solve, followed by prepare, process, analyze, share, and finally, act.
## Ask
1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?
## Prepare
The data for this project can be accessed at the following link : [Cyclistic Dataset](https://divvy-tripdata.s3.amazonaws.com/index.html)

This dataset contains data on Cyclistic users, both members and casual users, including rental start time, rental end time, type of bike used, and other details. For this project, I used data from January 2021 to December 2021. The data is stored in CSV format and will be combined to facilitate the analysis process.

Check the data quality using the ROCCC principle:
- Realiable: From the initial observation, there are data entries with Null values.
- Original: The data used comes from a first party, Motivate International Inc. (under this [License](https://divvybikes.com/data-license-agreement)), and does not involve any second or third-party data.
- Comprehensif: The data is sufficiently complete to address the business tasks.
- Current: The data is somewhat outdated, as it is from three years ago.
- Cited: The data is sourced from a first party.

## Process
`[For more details regarding the process, analyze, and share, please refer to the notebook.]`

This project conducted using `Google Colaboratory`. 

First, the dataset is loaded. After the data is successfully loaded, the data is merged. Next, data cleaning is performed by removing records with Null values, considering that the dataset is large enough that removing a small amount of data will not significantly impact the analysis, and filling in Null values would be difficult. Additionally, checks are made for duplicate data, and the data types of 'started_at' and 'ended_at' are converted to Datetime (due to incorrect formatting). Feature engineering is performed by creating the 'ride_length' feature, which represents the rental duration,'ride_length_second', and 'day_of_week' for analysis purposes and to answer the business task later. A check is conducted for the 'ride_length_second' feature, revealing erroneous data where the rental duration is less than 0, so the data will be filtered accordingly.

## Analyze
Analysis was conducted by examining the characteristics of the data, such as the average 'ride_length_second', the distribution of member and casual users, the average bike usage per day, and the number of member and casual bike users per day. This analysis was performed to address the business task.

## Share
The results of the analysis were then visualized (visualizations were created using the Matplotlib library) in the form of line charts, bar charts, and other diagrams. Insights were also extracted for each visualization.

Insights obtained:
- number of member riders is higher than casual riders. But, asual riders have a higher average ride length than member riders. The possible reason is that the ride length for rider members is less than casual riders, maybe because of frequency of rides. For member they typically use the bike-sharing service for commuting or short, frequent trips. They might ride for shorter distances but do so more often. While casual riders, may use the service for longer rides or leisure activities.
- Typically member and casual riders has same patern with the lowest number of rides is on cold month (Desember, January, and February), start to increase on March and the reah peak on warm month (June, July, August).
- Member riders usually use cyclistic on weekday, maybe they are worker or student who use cyclistic to go to work or school. Differ from casual riders who use cyclistic usually on weekend, maybe it's people who use cyclist to have fun during their holidays weekend.
- There is interesting patern which is spike during 7-8 o'clock and 16-18 o'clock "the rush hour" of office worker in member riders. The spike does'nt appear on cassual riders. This finding makes clear now that member riders use cyclistic bikes to commute to their workplaces, while casual riders use it for recreational purpose.
- casual riders prefer to use docked bike rather than member riders, because they are easier to find and don't require a subscription or membership. They might choose docked bikes for one-time or short-term use. Members are typically regular users who benefit from the flexibility and convenience of undocked or dockless bikes. These bikes can be picked up and dropped off almost anywhere, which is more convenient for daily commuting or frequent use. Also classic bike is type of bike that most popular among member and casual rider, this data can be important for future marketing.

# Act
Top 3 recommendations based on analysis:
1. Make special offers such as weekend pass membership to attract more casual riders to buy membership.
2. More focus marketing on warm month (June, July, August) especially for digital marketing to attract casual member like tourist to buy membership.
3. Implement seasonal discounts during the colder months (December, January, and February) to boost rentals during these periods of lower demand.

# Data Analisis Sales
Bekerja sebagai tim untuk melakukan analisis dan membuat visualisasi terhadap data sales (merupakan tugas pada UPI Summercourse 2024)

# Human Development Index Classification
Tugas akhir pada mata kuliah Data Mining and Warehouse. Melakukan analisis terhadap berbagai data, seperti data ketidakcukupan pangan yang nantinya ditentukan data apa saja yang akan digunakan sebagai data untuk membangun model klasifikasi IPM (Index Pembangunan Manusia)
