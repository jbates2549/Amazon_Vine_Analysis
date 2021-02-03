# Amazon_Vine_Analysis
Amazon ETL and bias analysis

## Overview
This analysis examines Amazon appliance reviews using Google Collaboratory, Apache Spark and Postgress SQL.  In this analysis we take Amazon review data, create and SQL database and analyze the data using Apache Spark. 

## Analysis

### Review analysis and 5-Star reviews

This analysis takes counts of appliance reviews with over 20 upvotes and counts the number of 5-star reviews.

First we create a dataframe and take the count of all reviews with over 20 upvotes.

![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/total_reviews.PNG)
Here we see that our total count of reviews is 5,030.

Next we create a dataframe with only vine reviews.

![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/vine_review_count.PNG)
In this dataframe we see that there are 35 vine reviews.

We further refine the reviews taking only 5-star reviews.

For non-vine reviews we have 1,963 5-star reviews.
![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/non_vine_5star_reviews.PNG)

For vine reviews we see that there are 18 5-star reviews.
![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/vine_only_5star_reviews.PNG)


### Summary

From our analyis we can note the following:


* 51% of vine (paid) reviews, totaling 18, are 5-star reviews.
* 39% of non-vine (unpaid) reviews, totaling 1,963, are 5-star reviews.
* It appears there there could be positivity bias given the higher percentage of 5-star reviews for the vine group.
* The sample size for vine reviews is small.  We should seek additional reviews to have a better sample size.


![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/percent_vine_reviews_5stars.PNG)


![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/percent_non_vine_reviews_5stars.PNG)


The following table summarizes our analysis of the appliance reviews.
![image_name](https://github.com/jbates2549/Amazon_Vine_Analysis/blob/main/summary_all_reviews.PNG)


We can perform the analysis of vine vs non-vine reviews for other products to determine the general trend for postivity bias.  Taking the average bias, we can normalize our results in this category to provide a more accurate rating for the appliance category.


