# M16-Amazon_Vine_Analysis

dataset link selected for this analysis: 
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Outdoors_v1_00.tsv.gz

## Overview 

The purpose of this project is to analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products
We used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. 

## Results: 
### The total number of reviews

<img width="616" alt="total reviews" src="https://user-images.githubusercontent.com/91625564/152715334-ee5a00ce-ad8b-4b7b-a9d7-5507c2f45077.png">


### Total 5 stars Vine reviews 

<img width="783" alt="vine 5 stars reviews" src="https://user-images.githubusercontent.com/91625564/152715381-d39014f5-6bc4-4ab9-b4b6-323e10bba3f2.png">


### Total 5 stars non-Vine

<img width="883" alt="non-vine reviews" src="https://user-images.githubusercontent.com/91625564/152715513-3cb56957-d564-43e2-8a6d-4948d967ce61.png">


### Percentage of 5 stars Vine reviews  

<img width="883" alt="vine 5 stars reviews percentage" src="https://user-images.githubusercontent.com/91625564/152715390-cb50279c-0506-45a5-ad1f-35d8f0b2926e.png">


### Percentage of 5 stars non-Vine reviews 

<img width="883" alt="non-vine 5 stars review percentage" src="https://user-images.githubusercontent.com/91625564/152715470-9cf41191-aee9-4ae8-acdf-6fa5e9d4200b.png">


## Summary: 

In summary, the results shows that that the bias is equal between Vine reviews and non-Vine reviews. The percentage of 5 stars reviews for Vine is 52% similar to the non-Vine reviews. But if we compare the total number of non-Vine reviews to the vine reviews, we can see that the numbers are significantly different. 39869 reviews were out of the program. This will lead us to conduct future analysis to help understand why majority of the reviewers were not vine. We can use split to compare the Vine 5 stars reviews to similar portion or non_vine 5 stars reviews. 


