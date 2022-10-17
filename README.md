# Amazon_Vine_Analysis

## Overview of the analysis of the Vine program:

With the experience of the SellBy project, now we were tasked with a larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products.

For this project, we choose the beauty database which contains reviews of a specific products, for this project we use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 

In the follow sections, we present the main results of the Vine program, including the reviews of the members of the program and the non-members, this to have a close analysis of the efficiency of the program.

## Results:

After sorting and filter the data, we got the Vine members and non-members: 
### Vine members:

![Grafica1](https://github.com/raulesqueda/Amazon_Vine_Analysis/blob/0f2a149770b6f0d50ac30d7779d11fbb21c0450a/Images/grafica1.PNG)

### Non-Vine members:

![Grafica2](https://github.com/raulesqueda/Amazon_Vine_Analysis/blob/0f2a149770b6f0d50ac30d7779d11fbb21c0450a/Images/grafica2.PNG)

With this data, we answer the following questions:

1.	How many Vine reviews and non-Vine reviews were there? 
	
The Vine members reviews were 647, in contrast, the non-Vine reviews were 74,113 (114 times the number of the Vine members).

2.	How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

In the same way, the Vine members reviews with 5 stars were 229, for the non-Vine reviews with 5 stars were 43,217 (189 times the number of the Vine members).

3.	What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Finally, the percentage of the Vine members reviews with 5 stars results in 35.39%, the percentage of non-Vine reviews with 5 stars were 58.31%.

The following images summarize the calculations we did for the data.

### Vine members:

![Grafica3](https://github.com/raulesqueda/Amazon_Vine_Analysis/blob/0f2a149770b6f0d50ac30d7779d11fbb21c0450a/Images/grafica3.PNG)

### Non-Vine members:
 
 ![Grafica4](https://github.com/raulesqueda/Amazon_Vine_Analysis/blob/0f2a149770b6f0d50ac30d7779d11fbb21c0450a/Images/grafica4.PNG)

## Summary:

As a summary, we want to state if there is any positivity bias for reviews in the Vine program, in the case of the beauty data, we can’t confirm there is a bias in the information, because the low percentage of the Vine members review with 5 stars in contrast with the non-Vine program members that result higher. In the case of beauty, there is more factors for these reviews, for example, the brand, advertisement, etc. 

As an additional analysis we could develop a code to analyze the product_title to know the exact products who had a 5-star review and contrast between the two types of members.
