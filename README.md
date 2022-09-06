# Prosper_Loan_Analysis

## Introduction
> Prosper is a leading financial peer-to-peer lending company that provides a platform where borrowers and lenders interact. The peer-to-peer lending platform market has been booming recently.Through these platforms, hundreds of investors earn, while thousands of borrowers receive funding more quickly.Although these platforms offer credit scores and basic borrower information to ensure that tradings are conducted in a secure atmosphere, there are still thousands of consumers who run the risk of losing money.
 



## Dataset Overview
>The Prosper loan dataset comprises of 113937 loan entries with 81 attributes on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others, from the year 2009-2014. There are two main categories:

1. Borrower information: Basic attributes of the borrowers such as annual income, condition of employment, interest rate, loan status, etc.
2. Loan performance information: Metrics evaluating the risk associated with the loans such as Prosper score and bank card utilization, etc.

>Dataset has 81 columns which is too large for our analysis, we need to create a new dataframe to wearhouse columns that will be important to this particular analysis. Access data in each column and identify elements that need to be fixed, in order to create interesting and trustworthy analyses and visualizations.

# Summary of Findings

Prior to 2009, Credit Grade, a key indicator of credit risk for investors, was used by Prosper for profiling its client. This rate is based on the borrower's credit score as reported by an impartial credit reporting bureau. However, at the time, Prosper's lending performance was not very good. Prosper established a new credit risk gauge, the Prosper Rating, which was viewed as harsher credit criteria for borrowers, after being temporarily shut down on the request of the SEC and restructuring. Prosper's loan default rate has dramatically decreased, according to the new loan performance. This is evident from the increase in prosper loan from 25.5% before 2009 to about 74.5% there after.
Prosper Rating  ranges from HR to AA(high to low risk) with a large porportion of rating missing as proper relied soly on rating from independent rating agencies prior to July 2009. from the diagram above it is observe that category c has the highest amount of loan disbursement. this is inline with reality as category is medium risk and most investors are speculators.
Most borrowers on Prosper indicate to be Professional, Computer Programmer, Administrative Assistant, Executive, Teacher, Analyst... All those people have chosen to borrow on Prosper instead of going to the conventional way and borrow from their commerciaL bank. This is could be due to an attractive interest rate offered for this categories of people.
Proper currently has about 67% of its loan still running and 23.2% completed. However, about 8% of Prosper's loans were charged-off or defaulted. Moreover, the remaining 2.4% of loans has the status Past Due which is an aggregation of loan past due between 1 and 120 days.
Throughout my study, I discovered that the creation of this rating was a step in the right direction for Prosper because it enabled them to significantly reduce defaults that may otherwise result in bad debt.

From My analysis of some Multivariant Variables i noticed the following:
1. The multivariate analysis here revealed that Prosper applies more stringent credit requirements to customers who are in default (past due, charged-off payments) (higher interest rates). These individuals also have lower credit scores than those with high status.

2. It's also important to keep in mind that various rates are employed depending on maturities. In other words, rates for 5-year loans are often higher than rates for loans with other maturities, regardless of the prosper grade (with the exception of the E rating, which has rates the same for 3- and 5-year loans, and the HR rating).This is obvious; a longer duration increases the likelihood of a default.

3. Those with high ratings naturally pay the lowest prices, as is usually said. It's noteworthy that there are just three years' worth of loans in this dataset for HR ratings. In addition, loans that have been charged off or defaulted on often have borrower APRs that are higher than loans that have been completed or are currently in progress for all Prosper Ratings other than "A" and "AA" (good records). Last but not least, a better income and a collateral help to get a bigger loan amount. It is clear that having a property is important for getting a bigger loan.

# Key Insights for Presentation

From my analysis of the prosper data, i observed that since 2011, there hasn't been a major difference between the rates charged to homeowners and non-homeowners. This is a bit unusual as collaterl is a major backbone that lenders fall on in case of default.

# Reasources:
1. seaborn documentation
2. Prosper [Data Dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)
3. [Example Project Udacity](https://classroom.udacity.com/nanodegrees/nd002-alg-t2/parts/cd0016/modules/7e1817ca-5505-4583-b772-2e50d49a14a0/lessons/ls2240/concepts/c192c490-40b0-4667-b2df-592cb42eaef8)
4. [Statology](https://www.statology.org/)
