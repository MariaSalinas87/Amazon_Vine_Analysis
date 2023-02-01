# Amazon_Vine_Analysis


1.	Overview of the analysis: Explain the purpose of this analysis.

I was working with Jennifer on the Sellby project and was asked to do a larger project. I needed to analize amazon reviews written by members of the paid Amazon Vine program. The program is a service than allows manufacturers ad publishers to receive reviews for their products. I had access to many databases. I chose to work with the one that reviewed personal care appliances. 

Link https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Personal_Care_Appliances_v1_00.tsv.gz

I used Pyspark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data to pgAdmin. I also had to analyze if there was any bias toward favorable reviews from Vine members in my database. 

2.	Results: Using bulleted lists and images of DataFrames as support, address the following questions:

How many Vine reviews and non-Vine reviews were there?

There were 85981 Vine Reviews and 2901 non-vien reviews. 

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

There were 48897 Vine reviews that were 5 stars, and 2901 reviews that were non-vine

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Percentage Vine= 56.87%
Percentage non vine = 3.37% 

3. Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

According to my research and analysis there is a bias when it comes to the vine program. Users who are paid for their reviews and likely to give 5 stars to the product as opposed to those who are not paid. 

Deliverable 1 charts from PgAdmin

Review_id_table

 ![image](https://user-images.githubusercontent.com/112505962/215937140-21a4a3a1-e59e-491b-a108-68a0f5fc552e.png)

 ![image](https://user-images.githubusercontent.com/112505962/215937162-ae22065d-d93b-4f0a-8b01-682e69c5334b.png)



Customer_table

 ![image](https://user-images.githubusercontent.com/112505962/215937179-bba03557-e4f4-4eb7-86ca-a3c0d2af9106.png)

![image](https://user-images.githubusercontent.com/112505962/215937205-31e2930c-5ebe-4bdf-a74e-af6db2790758.png)



 

Vine_Table

 ![image](https://user-images.githubusercontent.com/112505962/215937220-ac96faf6-d495-4382-a5a5-1f96a4bfb1f2.png)


 ![image](https://user-images.githubusercontent.com/112505962/215937236-18768ccb-5ee7-4827-bca9-9e04e500bf10.png)


Products_table
 
![image](https://user-images.githubusercontent.com/112505962/215937253-45b3bad6-0b66-49b6-9f4c-71be7b8f76d5.png)

![image](https://user-images.githubusercontent.com/112505962/215937261-de5b9cdb-ce73-4199-85a2-3555b8009f76.png)



