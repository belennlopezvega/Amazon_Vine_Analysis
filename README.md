# Amazon Vine Analysis

## Overview of Analysis

The purpose of this analysis is to analyze Amazon reviews for Personal Health Care Products written by members of the Amazon Vine program. To do this, we gathered the Personal Health Care Products data and used PySpark to extract the dataset, transform the data, connect to an AWS RDS, and then load the data into pgAdmin. We then used PySpark again to determine if there is any bias toward favorable reviews from Vine members. 


## Results

For reference and as an overview of the contents, the image below contains the first 20 rows of the table from which the data gathered from to get our results.

![This is an image](https://github.com/belennlopezvega/Amazon_Vine_Analysis/blob/main/helpful_votes_table.png)

Our technical analysis is shown below: 

![This is an image](https://github.com/belennlopezvega/Amazon_Vine_Analysis/blob/main/results.png)

Below are the findings we've submitted to the SellBy stakeholders:

#### Vine Reviews and Non-Vine Reviews

* There were 497 Vine reviews
* There were 120,863 non-Vine reviews

#### 5 Star Vine Reviews and Non-Vine Reviews

* There were 220 5 star Vine reviews
* There were 74,470 5 star non-Vine reviews

#### Percentage of 5 Star Vine Reviews and Non-Vine Reviews

* The percentage of 5 star Vine reviews out of all the Vine reviews is 44%
* The percentage of 5 star non-Vine reviews out of all the non-Vine reviews is 62%


## Summary 

Out of the 121,360 total reviews, a miniscule percentage were reviews coming from the Vine program. Looking at our percentages, there is some variance where products reviewed by Vine members have a statistically lower number of 5-star reviews when compared to total Vine reviews as it's at 44%. Where products reviewed by non-Vine members have a statistically higher number of 5-star reviews when compared to non-Vine reviews where it sits at 62%. However, both numbers are fairly close to 50% therefore bias isn't as strong. Given that paid Vine members are more likely to give more thorough reviews we conclude that there is no bias for reviews in the Vine program. To support our statement, we recommend totaling the number of 1 star Vine and non-Vine reviews to run the tests above and compared the results from our 1 star and 5 star Vine and non-Vine reviews. 
