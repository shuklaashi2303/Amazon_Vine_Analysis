# Amazon_Vine_Analysis

# Overview

This project analyzes Amazon Vine program and determines if there is a bias toward favourable reviews from Vine members.
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.
We focused on the US reviews for video games.

# Results

We worked on two of the google cola notebooks to get the vine analysis. First we worked on amazon review ETL and the tables derived from this notebook customers table, review id, vine and products tables. The tables actually imported through connection of database instance to sql pgadmin as per screenshot below:

<img width="1440" alt="Screen Shot 2021-06-20 at 3 11 36 PM" src="https://user-images.githubusercontent.com/79673185/122686657-4e366800-d1e0-11eb-9487-0d89382c5b69.png">
<img width="1440" alt="Screen Shot 2021-06-20 at 3 12 04 PM" src="https://user-images.githubusercontent.com/79673185/122686673-7625cb80-d1e0-11eb-9f16-c589816a2744.png">
<img width="1440" alt="Screen Shot 2021-06-20 at 3 12 19 PM" src="https://user-images.githubusercontent.com/79673185/122686678-7aea7f80-d1e0-11eb-8f49-a28c4cf91fca.png">



Now, the vine review analysis we need to get the total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews           

<img width="1440" alt="Screen Shot 2021-06-20 at 3 47 16 PM" src="https://user-images.githubusercontent.com/79673185/122686740-c7ce5600-d1e0-11eb-8eb8-ffe7892c5e88.png">
<img width="1440" alt="Screen Shot 2021-06-20 at 3 47 22 PM" src="https://user-images.githubusercontent.com/79673185/122686741-ca30b000-d1e0-11eb-898b-88459b00bcf7.png">


<img width="1440" alt="Screen Shot 2021-06-20 at 3 46 18 PM" src="https://user-images.githubusercontent.com/79673185/122686725-ba18d080-d1e0-11eb-861a-ca4612bfb6e2.png">


# Summary

51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program.
Additionally we could analyze the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.
