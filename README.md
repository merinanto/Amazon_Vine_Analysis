# Amazon_Vine_Analysis
## Overview of the Analysis
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.SellBy need to do analyis whether is there any bias toward favorable reviews from Vine members.

Analysis is done on the dataset:-https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Grocery_v1_00.tsv.gz

## Results

### Tools & Scripts  Used for Analysis

PySpark  is used to perform the ETL process 

1.to extract the dataset
2.transform the data 
3.connect to an AWS RDS instance
4.load the transformed data into pgAdmin

ETL process is updated in the script:- https://github.com/merinanto/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb

Vine Analysis is updated in the scrit:- https://github.com/merinanto/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb

### Output

Total Helpful Vine Reviews count :-61

Total Helpful NON Vine Reviews count  :- 28174

Total Helpful Vine review with five star rating count :- 20

Total Helpful NON Vine review with five star rating count :- 15672

Percentage of Vine reviews with 5 stars :- 33 %

Percentage of NON Vine reviews with 5 stars :- 56 %

## Summary

From the percentage of analyis helpful vine reviews with 5 star accounts for 33% while non vine helpful reviews with 5 star accounts for 56%.
Paid vine reviews are having negative impact than non paid reviews.Also 61% of non vine/paid reviews are verified purchases while only 1.6% of paid 
vine reviews are verified purchases . As buyers has general tendency to rely on verified purchases , non paid reviews will be considered more.
Overall looks like paid vine reviews are not helping much for Grocery sales.









