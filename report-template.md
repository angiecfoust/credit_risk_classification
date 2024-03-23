# Module 12 Report Template

## Overview of the Analysis

In this challenge, a logistic regression model was created to help identify the creditworthiness of borrowers. The regression model was
applied to data that included a variety of loan information including loan size, interest rate, debt to income ration, count of deragatory
accounts, a total debt count, and current loan status. The current loan status was the prediction goal- a '0' being a healthy loan and a '1'
being a high-risk loan.
#####
After reading the csv file, the target (loan status) and features (remaining columns) were set. Then the data was split 75%/25% into training and testing data, respectively. From there a logistic regression model was created, fit, and then predictions made.


## Results

A confusion matrix was generated for the data which showed the following results:

* 18679 true negatives, 80 false negatives (0.004%)
* 67 false postivies, 558 true positives (12%)

A classification report was also generated which showed a 99% accuracy score. The breakdown for healthy loans (0) and high-risk loans (1) is:
* Healthy loans (0)
    * Precision: 1.00 (this isn't truly 100%, but rounds to that)
    * Recall: 1.00
    * F1-score: 1.00
* High-risk loans (1)
    * Precision: 0.87
    * Recall: 0.89
    * F1-score: 0.88

## Summary

In summary, the logistic regression model works well with this data set, although it should be noted there were significantly fewer high-
risk loans in the data set than healthy loans (625 compared to 18,759) and this could cause inflated classification scores for healthy
loans. I do recommend this model with the caveat that periodic retesting take place as more data is available down the line.

