# Bank-Lending-Club-Keras-Tensorflow-Loan-Prediction
These files contain complete loan data for all loans issued through the 2007-2015, including the current loan status (Current, Late, Fully Paid, etc.) and latest payment information. The file containing loan data through the "present" contains complete loan data for all loans issued through the previous completed calendar quarter. Additional features include credit scores, number of finance inquiries, address including zip codes, and state, and collections among others. The file is a matrix of about 890 thousand observations and 75 variables. A data dictionary is provided in a separate file.

![download (10)](https://user-images.githubusercontent.com/57037068/83354391-69ca9880-a369-11ea-810f-51df058d30a2.png)

## # Imbalanced data - Classification problem data is not balanced
# Means that our accuracy will not be the main metrics that we will be looking for where while model will overfit to the Fully paid status, while underfit for charged off people
# Precision and recall (F1 score) will be the main representation for the "accuracy" of the model in the end


![download (9)](https://user-images.githubusercontent.com/57037068/83354393-6b945c00-a369-11ea-9910-7ab2309c9008.png)

![download (8)](https://user-images.githubusercontent.com/57037068/83354394-6cc58900-a369-11ea-977b-007b86f4df84.png)


![download (7)](https://user-images.githubusercontent.com/57037068/83354398-6df6b600-a369-11ea-9831-236f8a326099.png)

![download (6)](https://user-images.githubusercontent.com/57037068/83354399-6fc07980-a369-11ea-9e3f-91a62552885e.png)

![download (5)](https://user-images.githubusercontent.com/57037068/83354400-70f1a680-a369-11ea-9c14-43a40049c865.png)


loan_amnt	The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
term	The number of payments on the loan. Values are in months and can be either 36 or 60.
int_rate	Interest Rate on the loan
installment	The monthly payment owed by the borrower if the loan originates.
grade	LC assigned loan grade
sub_grade	LC assigned loan subgrade
emp_title	The job title supplied by the Borrower when applying for the loan.*
emp_length	Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years. 
home_ownership	The home ownership status provided by the borrower during registrationÂ or obtained from the credit report.Â Our values are: RENT, OWN, MORTGAGE, OTHER
annual_inc	The self-reported annual income provided by the borrower during registration.
verification_status	Indicates if income was verified by LC, not verified, or if the income source was verified
issue_d	The month which the loan was funded
loan_status	Current status of the loan
purpose	A category provided by the borrower for the loan request. 
title	The loan title provided by the borrower
zip_code	The first 3 numbers of the zip code provided by the borrower in the loan application.
addr_state	The state provided by the borrower in the loan application
dti	A ratio calculated using the borrowerâ€™s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrowerâ€™s self-reported monthly income.
earliest_cr_line	The month the borrower's earliest reported credit line was opened
open_acc	The number of open credit lines in the borrower's credit file.
pub_rec	Number of derogatory public records
revol_bal	Total credit revolving balance
revol_util	Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
total_acc	The total number of credit lines currently in the borrower's credit file
initial_list_status	The initial listing status of the loan. Possible values are â€“ W, F
application_type	Indicates whether the loan is an individual application or a joint application with two co-borrowers
mort_acc	Number of mortgage accounts.
pub_rec_bankruptcies	Number of public record bankruptcies
