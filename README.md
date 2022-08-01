 - NOTE: The database has been removed from AWS and is no longer available.

# Amazon Vine Analysis
This analysis uses PySpark to perform the ETL process to extract Amazon product dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Then uses PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Results: 
![https://raw.githubusercontent.com/kwarzeski/Amazon_Vine_Analysis/main/counts.png](https://raw.githubusercontent.com/kwarzeski/Amazon_Vine_Analysis/main/counts.png)
- There were 1207 Vine reviews and 97839 non-Vine reviews.
- 509 Vine reviews were five stars and 45858 non-Vine reviews were five stars
- 42.17% of Vine reviews were five stars and 46.87% of non-Vine reviews were five stars

## Summary: 
There is some bias in positive non-Vine reviews. 46.87% of non-Vine reviews were five stars, which is greater than the 42.17% of Vine reviews that were five stars. I would propose an analysis comparing whether Vine reviews are more helpful than non-Vine reviews.
