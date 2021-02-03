# Amazon_Vine_Analysis
Amazon ETL and bias analysis

## Overview
This analysis examines Amazon appliance reviews using Google Collaboratory, Apache Spark and Postgress SQL.  In this analysis we take Amazon review data, create and SQL database and analyze the data using Apache Spark. 

## Analysis

### Review analysis and 5-Star reviews

This analysis takes counts of appliance reviews with over 20 upvotes and counts the number of 5-star reviews.

First we create a dataframe and take the count of all reviews with over 20 upvotes.

![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/total_reviews.PNG)

Next we create a dataframe with only vine reviews.

![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/vine_review_count.PNG)

We further refine the reviews taking only 5-star reviews

For non-vine reviews
![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/non_vine_5star_reviews.PNG)

For vine reviews
![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/vine_only_5star_reviews.PNG)


### Summary

![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/percent_vine_reviews_5stars.PNG)


![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/percent_non_vine_reviews_5stars.PNG)


![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/summary_all_reviews.PNG)





