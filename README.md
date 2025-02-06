# Twitter Analytics (Interactive Dashboard Creation Using Msexcel)
## Project Objective
The twitter analytics are used to "Create a visual that shows the average engagement rate and total impressions for tweets posted between '01- 01-2020' and '30-06-2020'. Filter out tweets that received fewer than 100 impressions and like should be 0 and this graph should work only between 3PM IST to 5 PM IST apart from that time we should not show this graph in dashboard itself."

# DATA Set Used
- <a href="https://github.com/Kranthi-india/Twitter-Dashboard-Analytics-using-Powerbi/blob/main/Tweet%20Analytics%20Task%201.pbix">Dataset</a>

# Questions (KPI's)
1.What is the average engagement rate for tweets posted between 01-01-2020 and 30-06-2020?
2.What is the total number of impressions for tweets posted between 01-01-2020 and 30-06-2020?
3.How to filter out tweets with fewer than 100 impressions and likes as 0?
4.How to show the graph only between 3 PM IST and 5 PM IST?
5.How to visualize the data on the dashboard and exclude times outside 3 PM - 5 PM IST?

# Dashboard interaction
- <a href="https://github.com/Kranthi-india/Twitter-Dashboard-Analytics-using-Powerbi/blob/main/Tweet%20Analytics%20Task%201.pbix">View Dashboard</a>

## Process
1.Import your dataset that includes tweet details (date, impressions, likes, retweets, etc.).
2.Remove tweets with fewer than 100 impressions: Filter the dataset by Impressions >= 100.Remove tweets with 0 likes: Filter the dataset by Likes > 0.
3.In Power BI Query Editor, add a custom filter to keep only the tweets that were posted between 01-01-2020 and 30-06-2020.Filter: Date >= 01-01-2020 and Date <= 30-06-2020
4.Filter the data to include only records where the HourOfDay is between 15 (3 PM IST) and 17 (5 PM IST).
Example Filter: HourOfDay >= 15 AND HourOfDay < 17.
5.Average Engagement Rate:
Use the formula provided earlier to calculate the average engagement rate:-
AverageEngagementRate = DIVIDE(SUM([Likes] + [Retweets] + [Comments]), SUM([Impressions]), 0)
This will give you the average engagement rate of tweets posted during the given period.
Total Impressions:
Calculate the total impressions:-TotalImpressions = SUM([Impressions])
6.Create the Visual
7.Time-Based Display Logic
8.Publish to Power BI Service

## Dashboard
![image](https://github.com/Kranthi-india/Twitter-Dashboard-Analytics-using-Powerbi/blob/main/Tweet%20Analytics%20Task%201.pbix)

## Project insight
the average engagement rate and total impressions for tweets posted between '01- 01-2020' and '30-06-2020'
Filter out tweets that received fewer than 100 impressions = 4,157
Average enagagement rate = 0.02
tweets that received likes should be 0
graph should work only between 3PM IST to 5 PM IST 

## Conclusion
This project provides a detailed analysis of tweet performance for a specified period, allowing stakeholders to track engagement and impressions effectively. By filtering out low-impact tweets and limiting the display based on specific times, the dashboard ensures that only high-value, time-relevant data is presented, helping users focus on the most meaningful insights.

