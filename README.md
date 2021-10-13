# Amazon_Vine_Analysis

## Overview

The purpose of this analysis was to analyze reviews written via the Amazon Vine program and to try and determine if any bias towards positive reviews is present by Vine members.
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. For this assignment we were able to select a dataset from the Amazon Review Datasets https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt. 
I chose to further inspect the Video Games review dataset. 
With this dataset, I was able to complete this analysis using my knowledge of the cloud ETL process, PySpark, and pgAdmin.

## Results

The following images are used as reference in answering the questions of this section.

<img width="558" alt="Screen Shot 2021-10-12 at 8 48 23 PM" src="https://user-images.githubusercontent.com/86446641/137048153-4d6e44a2-1e0c-4da1-8809-d1547a497308.png">
<img width="634" alt="Screen Shot 2021-10-12 at 8 48 39 PM" src="https://user-images.githubusercontent.com/86446641/137048182-f34f2cc7-6581-4808-bb1e-eb6813218769.png">

- How many Vine reviews and non-Vine reviews were there?

There were 94 Vine reviews and 40,471 non-Vine reviews, totaling 40,565 reviews. 

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

Of the 94 Vine reviews, 48 of them were five-star ratings. Of the non-Vine reviews, 15,663 were five-star ratings. 

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

51.06% of Vine reviews were five-star ratings, while only 38.70% of non-Vine reviews were five-star ratings. 

## Summary

With these findings, there is certainly some credence that Vine revies may be more favorable than non-Vine. However, it would be wise to run an ANOVA test to see if these results are significant enough to reject a null-hypothesis that Vine results are equally or less favorable than non-Vine results. I think that this test would be especially wise considering the large disparity in numbers between Vine and non-Vine reviews. It would also be very interesting to see the disparity in five-star reviews for all the different databases available in Amazon Review Datasets https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt. If for each of these different datasets, there were a higher rate of five-star reviews from Vine reviewers than we would be quite certain that a bias is present in these reviews.

