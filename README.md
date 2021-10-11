# Amazon_Vine_Analysis

<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Amazon_Vine_Analysis/blob/main/Resources/1.PNG" /></p>

## Background
The work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

## Deliverable 1: Perform ETL on Amazon Product Reviews.

Using the cloud ETL process, you’ll create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (Links to an external site.), and extract the dataset into a DataFrame. You'll transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, you'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.


### The customers_table DataFrame
<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Amazon_Vine_Analysis/blob/main/Resources/customers_table.PNG" /></p>

### The products_table DataFrame
<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Amazon_Vine_Analysis/blob/main/Resources/products_table.PNG" /></p>

### The review_id_table DataFrame
<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Amazon_Vine_Analysis/blob/main/Resources/review_id_table.PNG" /></p>

### The vine_table DataFrame
<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Amazon_Vine_Analysis/blob/main/Resources/vine_table.PNG" /></p>

### All four DataFrames are loaded into their respective tables in pgAdmin
<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Amazon_Vine_Analysis/blob/main/Resources/2.PNG" /></p>


## Deliverable 2: Determine Bias of Vine Reviews

Using PySpark, Pandas, or SQL, you’ll determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis, you'll determine if having a paid Vine review makes a difference in the percentage of 5-star reviews

- There is a DataFrame or table for the vine_table data using one of three methods above 
- The data is filtered to create a DataFrame or table where there are 20 or more total votes
- The data is filtered to create a DataFrame or table where the percentage of helpful_votes is equal to or greater than 50% 
- The data is filtered to create a DataFrame or table where there is a Vine review 
- The data is filtered to create a DataFrame or table where there isn’t a Vine review 
- The total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews 


<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Amazon_Vine_Analysis/blob/main/Resources/3.PNG" /></p>
