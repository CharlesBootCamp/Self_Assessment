# Self_Assessment

I played the Circle role, which meant that I was in charge of the databases.

Using the following two Kaggle databases: 
https://www.kaggle.com/datasets/binduvr/pro-mma-fighters 
https://www.kaggle.com/datasets/rajeevw/ufcdata

I was able to break the data down into two separate CSV files which were then put into a pgAdmin SQL and joined together before being finalized and sent through Notebook in order to get it sent to the Machine Learning code. One CSV file contains the fight information for the UFC fighters, about 12k lines worth of data, and the other file contains the fighter information, especially their heights, weights, and their win/loss streaks. These two files were then loaded into pgAdmin SQL to go through AWS and a Notebook to be sent to the Machine learning section.

My teammates worked on creating the Machine Learning code that took in code going through the AWS and ended up having an average accuracy of the code ended up being around 61%.

Some challenges that we faced were trying to get the percentage of accuracy to a higher number, so we tried finding out the specific parts that influenced the data the most. The following parts were determined to be the most important ones:

avg_opp_SIG_STR_pct (Average Opponent Significant Strike %)
avg_SIG_STR_pct (Average Significant Strike %)
avg_opp_CTRL_time_seconds (Average Opponent Control time in seconds)
avg_CTRL_time_seconds (Average Control time in seconds
avg_opp_TOTAL_STR_landed (Average Opponent Total Strike landed)
avg_TOTAL_STR_landed (Average Total Strike landed)
avg_SIG_STR_landed (Average Significant Strike landed)
avg_opp_HEAD_landed (Average Opponent Head landed)
avg_HEAD_landed (Average Head landed)
avg_opp_TOTAL_STR_att (Average Opponent Total Strike attempted)

We were able to achieve the 61% after breaking the data down to focus on these specific parts based on the order of importance.
We were all also able to meet and in Slack and communicate outside of class to look at and examine how we all were doing, such as how we wanted to break down the CSV files and look at the Tableau heat maps.

We were able to find through the data that the average peak age of the fighters is between the ages of 30-34. As to be expected, each fighter can only take so much damage before their body gives into the hits, leading to focusing on certain parts, especially the avg_SIG_STR_pct. It was also found that the heights and reach of the fighters didn't matter; this is due to the UFC not relying too much upon these factors. Through the data found about the camps, even though the camps didn't create any noticable benefits, those without the camps did around 10% worse.

Ultimately, we were able to answer that Magomed Ankalaev would be the ultimate winner in the Title Fights and Alex Morono would do the best in the Catch Weight category. The was found by taking CSV files into an SQL and put through an AWS to go through Machine Learning. The Machine Learning code was able to finalize with a average accuracy of 61%, which isn't awful, but still leaves the capability for some improvement.
