# Market Basket Analysis for RM Customer Purchase Behavior

**Overview**

This project conducts a market basket analysis of customer purchase behavior using transactional data captured through RM's loyalty card system. The study focuses on understanding associations between bread, jelly, and peanut butter purchases, aiming to provide insights for pricing strategies, display optimizations, and coupon discount impacts.


**Project Objectives**

•	Create a binary transaction matrix from the transactional data.

•	Identify frequent itemset and association rules among bread, jelly, and peanut butter.

•	Provide recommendations to RM based on the insights derived from the analysis.


**Data Description**

The dataset (marketbasket.xlsx) provided by RM's Information Technology group contains purchases by 1000 customers over a one-week period. Each customer's purchase behavior is recorded with variables indicating the type of bread (wheat, white, or none), jelly (grape, strawberry, or none), and peanut butter (creamy, natural, or none).


**Tasks and Deliverables**

A) Creating a Binary Transaction Matrix
The R script reads the dataset, preprocesses it by converting variables to factors, and creates a binary transaction matrix where:

•	1 indicates the purchase of a product.

•	0 indicates no purchase.

The resulting matrix is then saved as a tab-delimited text file (marketbasket_binary_transaction_matrix.txt).

B) Initial Study and Recommendations
  1.	Market Basket Analysis
       
    o	The arules package is utilized to convert the preprocessed data into transactions.
    
    o	The Apriori algorithm is applied to mine association rules with a minimum support of 0.1 and minimum confidence of 0.6.
    
    o	Association rules are ranked by lift to identify significant product associations.
  
  2.	Recommendations
     
    o	Based on the top association rules, recommendations are provided to RM. By understanding which products are frequently purchased together, RM can strategically optimize its sales strategies         and enhance customer satisfaction.


Prerequisites

•	R programming language

•	Required R packages: readxl, arules


