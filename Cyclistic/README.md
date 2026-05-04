# 🚲 Cyclistic Case Study
## Project Overview
Working as a junior data analyst working on the marketing analyst team at Cyclistic, a bike-share company in Chicago, the director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members.
## Business Task
Explore how annual members and casual riders use Cyclistic differently, and give recommendations on converting casual riders in becoming members.
## Data Sources
The datasets used in this project are Divvy's trip data. The most recent 12 months of data were used. It includes:
- Ride IDs
- Type of bicycle (electric vs. classic)
- Start and end times of each ride
- Start and end stations of each ride
- Start and end latitudinal and longitudinal coordinates of each ride
- User type (member or casual rider)
## Tools
Python (pandas and matplotlib) for data cleaning, transformation and visualisation.
## Data Cleaning and Transformation
The 12 different CSV files were loaded and concatenated in Jupyter Notebook where I carried out data cleaning ad transformation prior to further analysis.
1. Converted 'started_at' and 'ended_at' from string format to datetime format.
2. Extracted the dates and time separately from 'started_at' and 'ended_at', as the data came compressed.
3. Created new columns, 'day_of_week' and 'ride_length' for analysis.
## User Data Analysis
Members and casual riders of Cyclistic were compared and analysed against these metrics:
- Average ride length
  - Average ride length on weekdays vs. weekends
- Average number of trips taken per day
- The peak times of rides taken

The purpose of analysing these specific metrics is to explore the key differences in usage of Cyclistic between members and casual riders, and cultivate new marketing strategies that build on these key differences to increase membership rates.
## Data Visualisation and Key Insights
Line graphs and bar charts were plotted using matplotlib on Python to highlight these key patterns and comparisons:
1. On average, casual riders cycle longer than members, an estimated 54% longer. This suggests that casual riders are more likely using Cyclistic for more leisure cycling, whereas members could be using it more for daily commuting to and fro work.
![Ride length](https://github.com/sashimiyuh/Bellabeat-Case-Study/blob/645dfcbdfac3ec1441d707608e46b253779cabf3/Cyclistic/Avg%20Ride%20Length.png)
3. This is bolstered by temporal riding patterns.
   - Ride times for members peak around typical work hours (7-9am and again at 4-6pm) whereas ride times for casual riders see a gradual increase throughout the day before peaking in the evening, suggesting leisure cycling outside standard working hours.
![Ride timing](https://github.com/sashimiyuh/Bellabeat-Case-Study/blob/51e55ff1518cad5cd338159b9935e508bb42a286/Cyclistic/Ride%20Timings.png)
   - Members on average take more trips than casual riders, despite riding for shorter amounts of time. This indicates that members have a more utilitarian approach when using Cyclistic, taking shorter but more frequent trips every day for commuting, while casual riders rely on Cyclistic for more recreational purposes.
![No. of rides per member](https://github.com/sashimiyuh/Bellabeat-Case-Study/blob/c677e2c922b40250a6b4a9f86d82783b44102e02/No.%20Rides%20per%20Member%20Type.png)
4. The number of rides taken on average, is higher on weekdays compared to weekends, for both members and casual riders. This reflects that in general, Cyclistic is seen and used by the public for structured weekday routines, and is seen as a reliable mode of transportation by both casual riders and members alike. 
   - Notably, the decrease in members riding on weekends is substantial compared to casual riders, with a 30.3% and 27.3% drop respectively. This is tied with the fact that ride durations are longer on weekends, further reinforcing the fact that Cyclistic's members are using it mainly for daily commute, while casual riders use it more leisurely and/or spontaneously.
![No. of rides](https://github.com/sashimiyuh/Bellabeat-Case-Study/blob/d4c0fabddca8f5f211108b46e9bb2216dc04a995/Cyclistic/No.%20of%20Rides.png)
## Recommendations
- Offer weekday-exclusive membership passes
  - Currently, Cyclistic offers single and full-day passes for casual riders. However, analysis has shown that casual riders do consistently use Cyclistic on the weekdays (even riding for longer than members), suggesting potential demand for a more flexible membership structure.
  - A weekday-exclusive membership lowers the barrier to entry to an annual membership (currently the only form of membership available at Cyclistic). This would allow users to test out the membership experience with Cyclistic within their existing riding patterns.
  - Overall, the goal would be to encourage a behavioural shift from a more leisurely usage, to every day commute, thus increasing annual membership rates.
  - _To encourage progression towards an annual membership, the weekday-exclusive membership could be priced such that repeated short-term use is less cost-effective than the annual membership. For example, purchasing multiple weekday passes over a month would cost more than monthly cost of an annual membership. This structure allows users to trial the weekday option initially, while creating a clear financial incentive to transition toward annual membership over time._
