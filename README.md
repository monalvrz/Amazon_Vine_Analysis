# Amazon_Vine_Analysis

## Overview of the analysis

This project seeks to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. 

Specifically, we worked with a database containing information about kitchen products. We used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Then we used PySpark to determine if there is any bias toward favorable reviews from Vine members in the kitchen dataset.

## Results
After working with the information contained in the database, we obtained the following data that allow us to perform an analysis of the possible bias in the vine program reviews:

### Total reviews 

<img width="274" alt="vine-reviews" src="https://user-images.githubusercontent.com/107893200/199136085-5aae2b25-65d2-4a9d-ae12-79e4d1a88479.png">

There are 1,207 reviews registered in the database that belong to the Vine program. 

<img width="220" alt="non-vine-reviews" src="https://user-images.githubusercontent.com/107893200/199136249-eb6caeca-e9a3-44f0-ac16-ab36dd5dd20f.png">

There are 97,839 reviews registered in the database that are non-Vine reviews.

### 5 stars reviews

<img width="344" alt="5stars-vineprogram" src="https://user-images.githubusercontent.com/107893200/199137006-8d089ae4-7348-4b8c-b0ab-edaa26c84588.png">

There are 509 reviews registered in the database that give the product 5 stars and belong to the vine program.

<img width="295" alt="5stars-nonvine" src="https://user-images.githubusercontent.com/107893200/199137206-54bcdcbd-2146-46a9-ac3f-fa14a8ed1a03.png">

There are 45,858 reviews registered in the database that give the product 5 stars that are non-Vine reviews.

### Percentage of reviews

<img width="551" alt="review-analysis-table" src="https://user-images.githubusercontent.com/107893200/199137702-7a37743a-d30f-4b14-a9e9-d507d5cb5cf2.png">

Based on the information presented above, the percentage of five-star reviews that belong to the Vine or non-Vine reviews were calculated. The 5-star reviews of the Vine program constitute 42% of the reviews, while the 5-star reviews of the non-Vine reviews constitute the 46%. 

## Summary 
