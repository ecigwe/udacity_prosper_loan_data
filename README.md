# Prosper Loan Data Exploration
## by Emmanuel Igwe


## Domain

Loan/Lending Analytics are the main subject of this analysis.

### objectives
1. Add visualizations to statistics to improve your understanding of the data.
2. To study a dataset and comprehend variable distributions and interactions between features, choose the right plots, limitations, transformations, and aesthetics.
3. Create excellent visualizations for presenting findings to an audience by applying design principles.
4. To comprehend the data, create univariate, bivariate, and multivariate graphs.
5. produce at least 15 exploration-related insights.

### Installation

The following libraries are used in this project:

NumPy
Pandas
Matplotlib
Seaborn

### Dataset

The dataset includes 114,000 rows of loan data with 81 different characteristics, including as loan amount, borrower income (stated monthly income), debt-to-income ratio, loan term, prosper score, and many more.
[more information about the dataset can be found here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)

### wrangling

1. A 20-column dataframe subset was produced.
2. Dataframe issues related to data quality and organization were evaluated.
3. Rows that lacked a Prosper Score were removed.
4. Using pandas' Categorical Dtype, ordinal categorical variables are transformed.
5. The words HomeOWner and Not Homeowner were used in place of True and False in the Is Borrower a Homeoner column. 
6. The dataset still contained 74,035 Prosper Loan listings with 20 variables.


## Summary of Findings

During my research, I discovered a positive relationship or correlation between the loan amount and the borrower's monthly income. I found that the chances of receiving a low or high loan amount are somewhat equal for borrowers with a low monthly income. The loan amount is higher when the monthly income is higher, though.


With the loan term having some modifying influence, there is a significant link between the monthly payments and the loan amount. The Visualization demonstrates that borrowers with longer loan terms (36 or 60 months) obtain greater loan amounts after encoding a bivariate plot with a third variable, the loan term.

Additionally, there was an intriguing connection between the categorical traits and the loan amount. Longer loan terms, low risk (high Prosper Score), home ownership, and gainful employment are all connected with more loans for borrowers.


## Key Insights for Presentation

For the presentation, I leave out the majority of the intermediate derivations and concentrate on the impact of the borrower's income (stated monthly income), monthly loan payment, loan length, and debt to income ratio on loan amount. I first introduce the Loan Amount variable, then I produce scatter plots to display correlations, and last I introduce the distributions of the other variables.

Loan amount and the predictor variable, stated monthly income, were correlated using scatter plots. The figure demonstrated that the odds of receiving both a low and high loan amount are comparable when an applicant has a relatively modest monthly income (less than $8000). However, a borrower is more likely to receive a large loan amount if their monthly income is substantial (>$8,000).

I then dug further deeper, producing multivariate scatter and point graphs to demonstrate that Loan Term affects the amount of loan to be granted. Additionally, the Prosper score has an impact (risk score). In other words, the larger the loan amount to be granted, the longer the loan term, and the higher the risk score (Prosper Score). This might be the result of lenders being more willing to extend credit to borrowers that they don't view as default risks and offering a lengthy repayment period as security for the huge loan amount.