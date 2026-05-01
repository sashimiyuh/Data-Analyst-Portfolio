# 💿 Bellabeat Case Study

## Project Overview
Working as a junior data analyst working on the marketing analyst team at Bellabeat, a high-tech manufacturer of health-focused products for women, focus on one of Bellabeat’s products and analyze smart device data to gain insight into how consumers are using their smart devices. The insights you discover will then help guide marketing strategy for the company.

## Business Task
Analyze smart device usage data in order to gain insight into how consumers use non-Bellabeat smart devices, then select one Bellabeat product to apply these insights to in your presentation.

## Data Sources
The dataset used in this project is the Fitbit Fitness Tracker Data, publicly available on Kaggle. It includes the:
- Daily Activity
- Steps
- Sleep Data
- Calories Burned of Participants.

## Tools
Python (pandas and matplotlib) for data cleaning, transformation and visualisation.

## Data Cleaning and Transformation
The CSV file was loaded into Jupyter Notebook where I carried out data cleaning ad transformation prior to further analysis.

1) Converted 'ActivityDate' from string format to datetime format.
2) Created a new column 'DayOfWeek' and reordered it within the dataset to improve readability and facilitate analysis.

🔗Link to script: [Bellabeat Analysis](https://github.com/sashimiyuh/Bellabeat-Case-Study/blob/main/Bellabeat/bellabeat_analysis.ipynb)

## User Data Analysis
I analysed user activity in the main dataset, which includes teps taken, activity intensity levels, and calories burned.

1) Average steps taken per day
2) Average calories burned per day
3) Average time spent on each intensity of exercise.

The purpose of this analysis was to understand overall user activity patterns and behaviour. In particular, how and why activity levels vary across the days of the week, and whether the weekend would play a part in affecting user behaviour.

Insights gained aim to support Bellabeat's marketing strategy by providing clarity on the existing pool of users using smart devices for fitness and health purposes, while identifying any potential gaps that Bellabeat could help fill. As such, this analysis will aid Bellabeat in making more informed decisions in targeting and engaging future users.

## Data Visualisation and Key Insights
Line graphs and bar charts were plotted using matplotlib on Python to highlight these key patterns and comparisons:


1) Average steps taken per day drop significantly from Mondays to Tuesdays, with an estimated 22% drop, before rising rapidly again from Tuesdays to Wednesdays, an estimated 26% increase. The fact of it being a weekday or weekend does not seem to affect the average step a user takes per day. When calculated, the average number of steps taken per day sits at 6610, not hitting the daily recommended average steps per day of 7000.



3) Average calories burned per day follows a similar pattern. Average calories burned per day drop from Mondays to Tuesdays, with an estimated 5.1% drop, before rising again from Tuesdays to Wednesdays, an estimated 6.35% increase. Similarly, the average calories burned per day does not seem affected by the weekday or weekend.
   
![Average calories burned per day](https://github.com/sashimiyuh/Bellabeat-Case-Study/blob/b52fb33cf50012ddf8de632761e3eb25f4104e9f/calories.png)

4) The intensity of activity users perform each day follow a descending order from 'Sedentary' being the most, followed by 'Light', 'Fairly', and 'Very Active' being the least time spent. It was found that even when the total active minutes of activity were calculated (sedentary is excluded), the amount of time users spend being sedentary still far exceeded the total active time spent.
   
5) A weak correlation was found between sleep and activity levels, suggesting other factors at play that for users' sedentariness.


## Recommendations
- Encouraging daily movement through in-app prompts and features.
  - Introduce features such as reminders to stand, stretch, or take short walks to reduce prolonged sedentariness and promote consistent light activity throughout the day. This aims to significantly lower time spent on sedentariness.
- Elements of gamification to increase user engagement.
  - Develop a gamified interface that allow users to set goals, earn rewards, and compete with friends. This can motivate users to increase their participation in moderate to high-intensity activities (e.g., “Fairly Active” and “Very Active” levels).
- Hosting community sports events to cultivate community engagement.
  - Organise team sports games or fitness challenges to encourage social interaction while promoting regular movement and fostering friendships between users.
