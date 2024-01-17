# Project Name: Lending Club Case Study
> Upon receiving a loan application, the business must decide whether to approve the loan based on the applicant's profile. Granting the loan could result in a loss of money for the company if the borrower is not likely to repay the debt, or if default is probable. The purpose of the analysis is to identify the crucial variables that are solid indicators of loan defaults so that those making decisions can minimize the likelihood of default risk by utilizing them to accept or reject loan applications.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information

### Project Background
> Consumer financing company that specializes in providing urban clients with a range of loans. Upon receiving a loan application, the business must decide whether to approve the loan based on the applicant's profile. Lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. If the lender is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss.

### Business Problem
> Assess the data and identify the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

## About Dataset
It contains the complete loan data for all loans issued through the time period 2007 t0 2011. If the loan requests from applicants were turned down by the company, then there will be no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)


## Conclusions
1) <span style='color:blue'>Top influencers</span> which can help to strongly decide if the loan applicant would default:
  - int_rate
  - term
  - composite_grade  (merging grade and sub_grade variables)
  - ratio_installment_to_funded_amnt_inv (ratio of Installment to funded_amnt_inv as these are correlated)
  - annual_inc
  - purpose
  - addr_state
  - delinq_2yrs
  - inq_last_6mths
  - pub_rec
  - pub_rec_bankruptcies
  - open_acc   (moderate impact)

2) <span style='color:green'>Correlated</span> influencers:
  - Installment and funded_amnt_inv
  - composite_grade and term
  - composite_grade and last_inq_6mths
  - term and last_inq_6mths
  - composite_grade and int_rate
  - ratio_installment_to_funded_amnt_inv and composite_grade
  - annual_inc and composite_grade 
  - term and purpose  (moderately correlated)
  - term and delinq_2yrs  (moderately correlated)


## Technologies Used
- Python - version 3.8.18
- pandas  - version 2.0.3
- numpy   - version 1.24.4
- matplotlib - version 3.7.4
- seaborn - version 0.13.1


## Acknowledgements
Give credit here.
- This research was motivated by IIIT-B, for the Machine Learning and Artificial Intelligence course


## Contact
Created by [@SoumitSarkar] - feel free to contact me!
