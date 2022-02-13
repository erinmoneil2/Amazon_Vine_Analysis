# Amazon_Vine_Analysis

## Overview
- The purpose of this analysis is to utilize PySpark, Amazon AWS, and PGAdmin, as well as the ETL process in order to analyze Amazon reviews written by members of the pain Amazon Vine Program. In this analysis specifically, we are looking to see if there is any bias toward favorable reviews from Vine members for a specific dataset. For this dataset, I utilized the Pet Products dataset. 

## Results 

### Vine Reviews for Pet Products
<img width="527" alt="Screen Shot 2022-02-12 at 9 08 13 PM" src="https://user-images.githubusercontent.com/92831268/153766902-9150c4ab-01c0-4358-a152-8c58d869c87f.png">

###Findings
- There were 170 Vine reviews and 37,823 non-Vine reviews.
- 65/170 Vine reviews received a 5-star rating. 
- 20605/37823 non-Vine reviews received a r-star rating. 
- 38.2% of Vine reviews received 5-star ratings. 
- 54.5% of non-Vine reviews received 5-star ratings. 

## Summary 
Since the percentage of Vine reviews receiving 5-star ratings was 38.2% and the percentage of non-Vine reviews received 5-star ratings was 54.5%, the non-Vine members had more favorable views than the Vine members. This would mean that there is no positivity bias within this dataset. We could conduct some additional analysis that may help with furthering this assessment by comparing the mean, median, and mode of all of the ratings across both Vine and non-Vine members. THe mean median and mode would help to indicate whether the Vine members or non-Vine members wrote more favorable reviews.  

