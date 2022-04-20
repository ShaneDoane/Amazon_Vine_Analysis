# Amazon_Vine_Analysis

## Overview
The purpose of this ETL & analysis is to determine if there is a bias in product review scores between Amazon Vine (solicited) and standard Amazon reviews.
Tools employed include: PySpark & Google Colab for data extraction and initial transformation, AWS & PostgreSQL for data load, and Pandas & Jupyter Notebook for final transformation and analysis. In this project, Amazon Grocery product [reviews](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Grocery_v1_00.tsv.gz) are analyzed.

## Results

* There were 61 Vine Reviews and 28,287 standard reviews 
* 20 (32.8%) of Vine Reviews were 5-star ratings
* 15,689 (55.5%) of standard Reviews were 5-star ratings

## Conclusions & Recommendations
There appears to, unexpectedly, be a negative bias for Amazon Vine reviews. Only 1/3 of reviews were 5-stars vs over 1/2 for standard reviews. One notable shortcoming is the sample size on Vine reviews, especially compared to the sample size of standard reviews. One additional component to add to this analysis would be to filter for verified purchases only in each Vine and standard datasets. This could eliminate fradulent reviews and provide a more trustworthy picture.
