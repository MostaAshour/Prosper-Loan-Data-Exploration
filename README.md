# (Prosper Loan Data Exploration)
## by (Mosta Ashour)
Using python and its internal libraries to explore the Prosper Loan Dataset.
Answering variety of questions by Univariate, Bivariate and Multivariate Exploration.


## Dataset

> This dataset is financial dataset and this is related to the loan, borrowers, lenders, interest rates and things like that.
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found in [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv),
with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).


## Summary of Findings

> In the exploration, I've checked the factors that can be associated with loan Status, so I've looked into the following variables(Term, BorrowerAPR, BorrowerRate, LenderYield, Occupation, listing category, Income Range, LoanOriginalAmount).
> The Term of the Loan was slightly correlated with the Loan Status since we could see that the highest percentage of Loan Defaulted was in the 3 years Term, with 12.36%.
BorrowerAPR, BorrowerRate, and LenderYield had a surprisingly high amount of correlation with the Loan Status, which we could see that Defaulted loans had a higher median than Completed ones.
There was also some important note, in income Range, borrowers who didn't displayed them Income range is more likely to Defaulted more than any income range.
>I extended my investigation of Loan Status against Stated Monthly Income and Loan Original Amount and by Time in this section by looking at the impact of the three categorical quality features.
The multivariate exploration here showed that there's a positive effect of increased in borrowers to complete with a high Stated Monthly Income by years.
It seems that the trend for different loan status is not the same across the years. so this can be used as a variable to get the profiles for defaulted and completed loans.
LoanOriginalAmount versus loanStatus and Term: For shorter loan 1 year term the Loan Status "Current" had the highest Loan Original Amount, Defaulted was the lowest. For 3 and 5 years Term, borrowers had a higher range of Loan amount, thought the longer term, the bigger Amount of Loan.
Current borrowers seems to get lower Loan term than longer.


## Key Insights for Presentation

> For the presentation, I focus on just the influence of the two Loan Status types,  and leave out most of the intermediate derivations. I start by introducing the LoanStatus variable, followed by the pattern in IncomeRange distribution, then plot the BorrowerAPR.

> Afterwards, I introduce each of the categorical variables one by one. To start, I use the violin plots and bar plot of LoanStatus and StatedMonthlyIncome across Years. I'm only looking at the Years plot here since it's the clearest example of how the Stated Monthly Income affect LoanStatus throw Years. The other two variables, LoanOriginalAmount and Term, are covered afterwards, using box plots. I've made sure to use different color palettes for each quality variable to make sure it is clear that they're different between plots.

