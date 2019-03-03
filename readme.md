# Financial Graveyard: Digging in to Failed Loans
## by Spencer McTavish


## Dataset - Prosper Loans

Prosper Loans is a company supplying individually backed loans to consumers throughout the US. The dataset they have shared includes 113,937 loans with 81 variables for each loan covering much of the data an interested lender would want. This data was updated as of 2014-Nov-03. 

The dataset offers comprehensive information gathered for each loan and a variety of ways to look at it. 




## Summary of Findings

* There's a (to me) surprisingly high failure rate amongst Prosper loans in this dataset. A 30.8% failures rate seems high, and suggests backing a Prosper loan is risky. 
* Credit Grades and Credit Scores follow as similar pattern of a bell-curve distribution until you get to the lower credit scores and grades, where there's a significant drop-off in people.
* Borrower APR and original loan amounts are all over the place. 
* Higher Borrower APRs show up more on failed loans. It suggests that there's a relationship between high APRs and failed loans.
* Completion rates are higher amongst people with better Credit Grades - unsurprisingly.
* People with better Credit Grades get better rates. Interestingly, people at High Risk and people in E category get similar treatment, whereas those with No Credit have some assumed average value. 
* Comparing mean APR for completed and failed loans shows an interesting difference across all of our grades - failed loans have a higher mean APR than those of completed loans, across most grades. When we get to higher risk categories, the APR values tend to converge.
* Lender yield, the measure of how much a lender is expected to get for a given APR, also corresponds with higher failure rates. We've accounted for the overall borrower APR being a factor by calculating the ratio between yield and Borrower APR . Higher ratios, more expected profit are associated with higher failure rates. 
* Higher yields are again apparent in our failed loans, again across the board. 
* Debt to Income ratios are only calculated on credit check, and appear to be a bad indicator of a loan failing or not.
* Amount of money left over after servicing a loan debt appears to be a good indicator of whether a loan will fail or not. There's a divergence in this variable after about $2000/mo left after loan payment that leads to loans that are more likely to succeed. 


### Assumptions
* CreditRating and ProsperRatings are equivalent. This hasn't been verified yet, but can be by comparing the Credit Scores against both of these to see a Prosper Rating and Credit Rating encompass the same bins. Not completing this exercise due to current time constraints.
> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.


## Key Insights for Presentation

The biggest insight was the apparent link between a failed loan and higher APRs. This was backed up by apparently higher investor yields for these loans. 

Is a push for a better return actually leading to higher loan failures? 