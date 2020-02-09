# Prosper Data Exploration
## by Hao Xu


## Dataset

Prosper is America's first peer-to-peer lending company. The data consisted 
81 loan features, including loan basic information (such as Borrower Rate, 
Loan amount, Loan Status), Pre-loan management infomation (such as borrower 
credit information, prosper rating and score, borrower income and de) and 
Post-loan information (such as loan status, principle outstanding) of 
approximately 112,000 Prosper loans. The dataset can be found [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554486256021000),
with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).



## Summary of Findings

I am most interested in how Prosper set the borrower's loan interest rate.
In the exploration, I found that there was a strong relationship between the
borrower rate of a loan and the borrower's Prosper rating, the relationship is
approximately linear. Term is also a important feature, it shows strong 
correlation with Borrower Rate. Besides those, features such as wether the 
borrower is homeowner, if income verified, borrower's inquiry and delinquency 
history all more or less affect the borrower rate.

Outside of the main variables of interest, I found most of the loans are less than
15000$, and are multiples of 500$. There is a abnormal aggregation around 31% borrow
rate, most of these loans have amount less than 7500, and have low Prosper ratings.
For borrowers with different Prosper Ratings, they have different loan amount ceilings.
Follow the timeline, I also found Prosper changed its requirement several times.


## Key Insights for Presentation

For the presentation, I focus on two questions: what are the basic requirements
for getting a loan, and what features are related to borrower rate.I start by 
introducing the Borrow Rate and loan amount variables, then plot the time series
features. I find Prosper change its mimimun credit score twices, and raise its
minimun and maxium loan amount, those can answer my first question.

Afterwards, I researched the possible features which may affect the borrower rate 
one by one. I first get the linear relationship between rate and prosper rating, 
then find a second most important feature, the term. At the last part, I looked 
into several cerdit related features, those features all effect the final borrower
rate base on the rate determined by Prosper Rating.
