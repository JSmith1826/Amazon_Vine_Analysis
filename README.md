# Amazon Vine Analysis
## This project uses Amazon Web Services to to host a database of kitchen product reviews

Amazon has a program called Vine where manufacturers pay Amazon a fee and customers receive free products. In return customers are expected to leave reviews for the free products on Amazon's site.

Because of the way product reviews drive sales on Amazon's platform there is a big incentive for manufacturers to get as many reviews for their products as possible.

The point of this analysis is to compare the percentage of 5 star ratings for reviews generated by the Vine program and those that came in naturally in an attempt to determine if the program is implicitly biased.

For the purpose of this analysis, we selected kitchen products as a market segment to analyze. 

### Resources
Python 3.10.5, Pandas 1.4.3, Spark 3.3.0, matplotlib 3.5.2, pgAdmin 6.7, Virtual Studio Code 1.70.1

## Questions

Over the course of this analysis, we will attempt to answer the following questions to attempt to assess the bias created by the Amazon Vine paid review programs:

- What is the proportion of Vine reviews to non-Vine reviews?
- How may five-star reviews are there in each subset of reviews (Vine vs Non)?
- What percentage of overall reviews are five stars for each subset?


## Results
### ETL Process Using AWS and PySpark

The data was extracted and loaded to Amazon Web Services in the Jupyter Notebook entitles Amazon_Reviews_ETL.ipynb

After the data was loaded onto the server the vine_table was outputted in to a csv file, named vine_table.csv the statistical analysis was conducted using that csv file

### Analysis

The data from the vine_table.csv file was analyzed in a Jupyter Notebook titled Vine_Review_Analysis.ipynb

The following are some of the findings

#### Total number of Reviews (Vine vs Not Vine):
![Total Reviews](/images/total_reviews.png)

#### Five Star Reviews (Vine vs Not Vine):
![Five Star Reviews](/images/five_star_reviews.png)

#### Five Star Percentage (Vine vs Not Vine):
![Five Star Percentage](/images/percentage_reviews.png)

## Summary

The percentage of five-star reviews for each subset (Paid reviews vs Unpaid reviews) is not significantly different. 

It does not appear that Amazon's Vine program does not bias reviews for the kitchen products category of Amazon's store.

