Social Media Engagement Analysis
Studies 5,000 social media posts to find out what makes a post get more engagement (likes, comments, shares).

Data

File: social_media_engagement_5000.csv

Each row is one post. It includes the post type, category, hashtags, country, device, user age and gender, follower count, impressions, watch time, sentiment, and the likes, comments and shares it received.

- Load the data – reads the CSV with pandas.
- Check the data – looks at size, data types, missing values and duplicates.
- Clean the data
Converts the date column to a real date format.
Removes repeated posts (same post_id).
Fills missing numbers with the median.
Fills missing gender and sentiment with "Unknown".
- Create new columns
total_engagement = likes + comments + shares
engagement_rate = total engagement ÷ impressions
Year, month, day of week, hashtag count, and age group
- Handle outliers – very high engagement rates are capped using the IQR rule, so a few extreme posts don't skew the results.
- Explore the data – compares average engagement by:
post type, category, country, device
verified vs. not verified accounts
sentiment and age group
day of the week and top hashtags
- Make charts – distribution, bar charts, correlation heatmap, followers vs. engagement, and a monthly trend line.
- Predict engagement 



Libraries used

pandas, numpy, matplotlib, seaborn, scikit-learn
