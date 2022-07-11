# Amazon_Vine_Analysis

## Overview:

The overall goal of this analysis was to review if there is any bias toward favorable Amazon reviews from Vine members in one of the 50 datasets available; I used the video game reviews dataset (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz). During this analysis I performed the ETL process to extract the dataset using PySpark, I created and connected to an AWS RDS instance, and I was able to load the transformed data into pgAdmin. From there I was able to export the data to a CSV and use Pandas to analyze and review if there appeared to be any bias in the dataset. 

## Results:
### 1. How many Vine reviews and non-Vine reviews were there?
In this dataset there were a total of 4,291 Vine(paid) reviews and 1,781,706 Non-Vine(unpaid).

### 2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
In this dataset there were a total of 1607 Vine(paid) 5 star reviews and there were a total of 1,025,317 Non-Vine(unpaid) 5 star reviews.

### 3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars? 
- Percentage of 5 star Vine reviews vs total reviews = 0.09%
![1]()
- Percentage of 5 star Vine reviews vs total 5 star reviews = 0.16%
![2]()
- Percentage of 5 star Vine reviews vs total vine reviews = 37.45%
![3]()
- Percentage of 5 star Non-Vine reviews vs total reviews = 57.41%
![4]()
- Percentage of 5 star Non-Vine reviews vs total 5 star reviews = 99.84%
![5]()
- Percentage of 5 star Vine reviews vs 5 star Non-Vine reviews = 0.001%


## Summary: 
After completing this analysis, I don't think there is any positivity bias for reviews in the Vine program. Just to start, the number of Vine reviews overall is very low, coming in at only 4,291 vs. the 1,781,706 Non-Vine reviews. Also, the 5 star vine reviews are only 37.45% of the total vine reviews and only 0.09% of the total reviews. The Non-Vine 5 star reviews come in at a much higher percent when comparing to the total review count, at 57.41%. 