# Amazon_Vine_Analysis

# Overview

This project analyzes Amazon Vine program and determines if there is a bias toward favourable reviews from Vine members.
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.
We focused on the US reviews for video games.

# Results

We worked on two of the google cola notebooks to get the vine analysis. First we worked on amazon review ETL and the tables derived from this notebook customers table, review id, vine and products tables. The tables actually imported through connection of database instance to sql pgadmin as per screenshot below:


Now, the vine review analysis we need to get the total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews                                                                                                                                                                                                                                       

# Summary

51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program.
Additionally we could analyze the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.