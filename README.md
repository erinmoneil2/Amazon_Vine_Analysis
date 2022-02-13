# Amazon_Vine_Analysis

## Overview
- The purpose of this analysis is to utilize PySpark, Amazon AWS, and PGAdmin, as well as the ETL process in order to analyze Amazon reviews written by members of the pain Amazon Vine Program. In this analysis specifically, we are looking to see if there is any bias toward favorable reviews from Vine members for a specific dataset. For this dataset, I utilized the Pet Products dataset. 

## Results 

Our first step was to create the same Vine_Table that we created in our Amazon_RDS analysis to show our review_ids, star_ratings, helpful_votes, vine, and verified_purchases. 

<img width="981" alt="Screen Shot 2022-02-13 at 9 59 43 AM" src="https://user-images.githubusercontent.com/92831268/153768286-0daa81f7-7dce-4b87-9dc0-4a7f9a4bf67c.png">

Next we needed to create a new Datafram where the total number of votes is equal to or greater than 20. 

<img width="1088" alt="Screen Shot 2022-02-13 at 9 59 58 AM" src="https://user-images.githubusercontent.com/92831268/153768307-372ae87d-add1-45be-9b55-b6206ac39683.png">

Our next step was to filter the data to retrieve the rows where the number of helpful votes divided by the total votes is equal to or greater than 50%. 

<img width="1303" alt="Screen Shot 2022-02-13 at 10 00 14 AM" src="https://user-images.githubusercontent.com/92831268/153768344-cbee2dd9-629f-4982-a9db-b078b04d9fd9.png">

Then we wanted to filter out all of the reviews for anyone that pays for the Vine program. 

<img width="824" alt="Screen Shot 2022-02-13 at 10 00 38 AM" src="https://user-images.githubusercontent.com/92831268/153768367-59ab5dae-92d3-40ad-b292-771b3dea9974.png">

Lastly, we filter for the reviews for non-Vine members. 

<img width="826" alt="Screen Shot 2022-02-13 at 10 00 59 AM" src="https://user-images.githubusercontent.com/92831268/153768396-f7cce9bd-b8ed-4d44-a94c-3c904c2963b9.png">

### Vine Reviews for Pet Products
<img width="527" alt="Screen Shot 2022-02-12 at 9 08 13 PM" src="https://user-images.githubusercontent.com/92831268/153766902-9150c4ab-01c0-4358-a152-8c58d869c87f.png">

### Findings
- There were 170 Vine reviews and 37,823 non-Vine reviews.
- 65/170 Vine reviews received a 5-star rating. 
- 20605/37823 non-Vine reviews received a r-star rating. 
- 38.2% of Vine reviews received 5-star ratings. 
- 54.5% of non-Vine reviews received 5-star ratings. 

## Summary 
Since the percentage of Vine reviews receiving 5-star ratings was 38.2% and the percentage of non-Vine reviews received 5-star ratings was 54.5%, the non-Vine members had more favorable views than the Vine members. This would mean that there is no positivity bias within this dataset. We could conduct some additional analysis that may help with furthering this assessment by comparing the mean, median, and mode of all of the ratings across both Vine and non-Vine members. THe mean median and mode would help to indicate whether the Vine members or non-Vine members wrote more favorable reviews.  

