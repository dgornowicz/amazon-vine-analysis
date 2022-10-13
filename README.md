# Amazon Vine Analysis

## Analysis Overview
This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.\
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.\
We focused on the US reviews for video games.

## Resources
- Data Source: [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), [Video Games Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
- Software: Google Colab Notebook, PostgreSQL 11.9, pgAdmin 4, AWS

## Results
### Total number of reviews
- Vine reviews <p align="center">
     
</p>
<img width="193" alt="total_reviews" src="https://user-images.githubusercontent.com/102050273/195716076-c3c96e55-f2f0-4f0d-a633-fb88fa5a735f.png">
<br>

- Non-Vine reviews <p align="center">
     
</p>
<img width="218" alt="unpaid_reviews" src="https://user-images.githubusercontent.com/102050273/195716110-712b85db-b3b2-43a4-b2f8-f7426980f5b6.png">
<br>

### Total number of 5-star reviews
- Vine reviews <p align="center">
     
</p>
<img width="365" alt="paid5star_reviews" src="https://user-images.githubusercontent.com/102050273/195716165-a50197c7-8f0a-4d73-9304-9cc499d24281.png">
<br>

- Non-Vine reviews <p align="center">
     
</p>
<img width="386" alt="unpaid5star_reviews" src="https://user-images.githubusercontent.com/102050273/195716201-f6f946fa-9a84-4634-b61e-a0ce83f19df4.png">
<br>

### Percentage of 5-star reviews
- Vine reviews <p align="center">
     
</p>
<img width="382" alt="paid5star_rate" src="https://user-images.githubusercontent.com/102050273/195716222-c458a218-70c2-4727-b4db-74c723d72c0a.png">
<br>

- Non-Vine reviews <p align="center">
     
</p>
<img width="412" alt="unpaid5star_rate" src="https://user-images.githubusercontent.com/102050273/195716243-3d98bbc0-d53d-47b8-a178-0ea9a44327e0.png">
<br>

## Summary
51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program.\
Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.
