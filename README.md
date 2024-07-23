# Lending Club Case Study
> The aim is to identify patterns that indicate if a person is likely to default, which may be used for actions such as denying the loan, reducing the loan amount, or lending at a higher interest rate. The goal is to identify these risky loan applicants to reduce credit loss using exploratory data analysis (EDA).


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.
  A consumer finance company [Lending Club] which specialises in lending various types of loans to urban customers. 

- What is the background of your project?
  When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile.
  Two types of risks are associated with the bank’s decision:
  If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
  If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

- What is the business probem that your project is trying to solve?
  Lending Club Platform needs insights to assess the risk in loan accept/reject to its customers based on the loans history data from 2007 to 2011 by identifying the driving factors for loan defaulters.

- What is the dataset that is being used?
  loans history data from 2007 to 2011.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
### Observations from Univariate Analysis:
- Loan Amounts: More defaulters are observed with loan amounts between 3k and 12k.
- Annual Income: Many defaulters have annual incomes between 2k and 8k.
- DTI Value: The number of defaulters increases with higher DTI values.
- Interest Rates: Defaulters are more common with interest rates between 10% and 18%.
- Loan Status: The distribution of loan status is consistent across loan amounts.
- Interest Rate for Defaulters: Defaulters have higher interest rates compared to fully paid loans.
- Homeownership: Defaulters are ranked as RENT > MORTGAGE > OWN > OTHER.
- Verification Status: Defaulters are ranked as Not Verified > Verified > Source Verified.
- Purpose: Debt consolidation is the most common purpose among defaulters.
- Employment Length: Defaulters with 10+ years of employment are notably high.
- Grade: Defaulters are ranked as B > C > D > A > E > F > G.
- Term: Defaulters with a 36-month term are more common than those with a 60-month term.
- Address State: CA has the highest number of defaulters, followed by FL, NY, TX, and NJ.
- Monthly Trends: The number of defaulters is increasing monthly.
- Yearly Trends: The number of defaulters is increasing yearly.

### Observations from Bivariate Analysis:
- Grades: Defaulters are predominantly in grades B and C. Subgrades B3, B4, B5, C1, C2, and C3 have the highest number of defaulters.
- Verification Status: Across all homeownership types, the "Not Verified" status is most common among defaulters. For RENT homeownership, defaulters are equally distributed between "Source Verified" and "Verified" statuses.
- Purpose: Debt consolidation is the most common purpose among defaulters across all homeownership types. For RENT homeownership, the second most common purpose is "other," while "home improvement" ranks second and "credit card" third for MORTGAGE homeownership.
- Employment Length: Defaulters with 10+ years of employment are most common across all homeownership types. For RENT homeownership, the second highest category is "< 1 year" and the third is "2 years," whereas for MORTGAGE homeownership, "3 years" ranks second and "5 years" third.
- Grades and Verification Status: For grades A to D, the "Not Verified" status is more common, while for grades E to G, the "Verified" status is more prevalent.
- Grades and Purpose: Across all grades, debt consolidation is the most common purpose. For grades A to D, the second most common purpose is "other," whereas for grades E to G, "small business" takes the second spot.
- Grades and Employment Length: Defaulters with 10+ years of employment are more common across all grades.
- Grades and Homeownership: Defaulters are more commonly associated with RENT and MORTGAGE homeownership.
- Verification Status by Employment Length: Across all employment lengths, the "Not Verified" status is more prevalent. However, for employees with 10+ years of experience, the "Verified" status is more common.
- Employment Length and Grades: Employment lengths of 1 year, 10+ years, 2 years, 4 years, 5 years, 7 years, and 8 years have more Grade B defaulters, while 3 years, 6 years, 9 years, and less than 1 year have more Grade C defaulters.
- State Observations: Verification status "Not Verified," employee lengths of 10+ years and less than 1 year, and homeownership "RENT" are prevalent across many states. Particularly in California (CA), RENT homeownership is the most common among defaulters.
- Interest Rates and Defaulters: As interest rates increase, the number of defaulters rises, regardless of annual income and loan amount. Defaulters are more common with interest rates of 12.5% or higher.
- Annual Income and Defaulters: Applicants with lower annual incomes are more likely to default compared to those with higher annual incomes.

### Observations from Multivariate Analysis:
- Loan Amount and Grade: The negative correlation between loan amount and grade indicates that lower loan amounts are associated with better grades among defaulters.
- Loan Amount and Annual Income: A correlation of 0.37 between loan amount and annual income shows a moderate positive relationship. This suggests that as annual income increases, the loan amount tends to increase as well, although the correlation is not very strong.
- Grade and Interest Rate: The strong positive correlation between grade and interest rate indicates that higher loan grades are associated with lower interest rates among defaulters.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Tools and Technologies Used
To run this project, you need to have Anaconda Jupyter Notebook and Python installed along with the following libraries:
- pandas
- numpy
- matplotlib
- seaborn
- warnings

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Created by [[@ramyaam](https://github.com/ramyaam)] [[@rajashekar52](https://github.com/rajashekar52/)] - feel free to contact us!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
