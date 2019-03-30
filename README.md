# AB_test
*AB test and logistic regressions to assess company web pages*

This project seeks to analyze the impact of an A/B test run by an e-commerce website. It calculates probability and runs A/B Tests and logistic regressions to help the company understand if they should implement the new page, keep the old page, or run the experiment longer to make their decision.

## Datasets
* ab_data.csv - conversion values for each user in the treatment and control groups 
* countries.csv - the users' country to account for possible regional differences in conversion rates
* Analyze_ab_test_results_notebook.ipynb - Python code for analysis
* Analyze_ab_test_results_notebook.html - HTML version of analysis

## Analysis

An A/B test and six logistic regression models were ran. One model, which included the interaction between weekday, suggests a statistically significant difference between the new and old pages (p-value=0.037). However, these results are not practically significant: Themagnitude of impact of the new page is negligeable as the exponent of the coefficient is slightly under 1, meaning the new page is slightly less effective.

## The verdict

The A/B tests and the logistic regressions all suggest that the new page would not be an improvement. Although looking at the interaction between whether the user viewed the new page or the old page on a weekday or weekend was statistically significant, it was not practically significant. The new page is slightly less effective but perhaps not different enough from the old page to learn from what customers like.
