# credit-loan-analysis
**Problem Statement:** To find the patterns, variables or driving factors in the data that will help avoid denying the loan to the applicants capable of repaying it.

**Design:**
1.	We have two types of data for analysis. One consists of current applicants, with details like what is their application status, loan credit amount, income, living situation, family status, assets they own etc. Other file consists of the previous application data of the applicant.
2.	The current applicant file has a variable Target, which takes values 0,1. 0 stands for people who have paid the loan and 1 for those you have difficulty is paying.
3.	All the applicants who have difficulty in paying the loan, have been grouped together in the dataframe called as defaulters and other have been grouped in dataframe called as repayers.
4.	I am doing the further analysis of the dataset by comparing other variables of the dataset with these features.
5.	Similarly for previous applications data we have 4 different categories based on the status of the loan – approved, cancelled, refused, unused offer.
6.	For the purpose of analysis, I have used the data with Approved and Refused status and compared the other variables w.r.t to these two categories.
7.	The previous application file also has the details of current application ID – which helps us understand how many times the user with the current loan application has previously applied for the loan and what was his status. 
8.	I have further segmented the data on this basis and tried to verify the findings derived from EDA.
9.	This has helped to understand what could be the driving factors giving the capable applicant the required loan.
10.	For all the categorical variables I have not replaced the missing values, because replacing them with the mode value would have created imbalance in the data.
11.	For the numerical variables, I have replaced the null values with mean value.

**Observation from EDA:**
1. Defaulters for revolving loans is less.
2. Applicants who have realty asset, but don’t have cars have defaulted.
3. Defaulters fall in the region with rating 2.
4. Overall living situation for defaulters is less than 15 and for repayers is more than 20.
5. Overall docs given by defaulters is less than 2, whereas for repayers it is at least 2-3.
6. Children count for repayers have outliers.
7. Comparison of annuity amount and credited amount tells that the defaulters have a steeper relationship compared to repayers.
8. The credit amount comparison with the goods price for which the loan is requested, suggest that repayers have outliers.
9. The overall credit bureau enquiries suggest that there are outliers in repayers.
10. The loan term offered to approved applicants have smaller range, but has more outliers.
11. Yield group for approved applicants is middle/high and for refused applicants is low/middle.

**Next Steps:**
1. Inorder to confirm the observations derived through EDA, I have created 2 subplots in the data with categories of applicants – Loan previously approved, but the applicant has turned defaulter, Loan previously refused but the applicant has turned repayer.
2. I then checked if the observations found in EDA are confirmed by these two subplots of the data.

**Conclusion:**
1. The current and previous application data is imbalanced. Distribution of its variables is skewed.
2. We were able to confirm few observations from the EDA.
3. We can conclude that person’s age, car and flat ownership, population density of the area in which they reside, overall living situation assessment, documents submitted - these variables could be considered as driving factors while identifying the applicants capable of repaying the loan.
4. Also in certain cases we have observed that outliers where the applicant has re-payed the loan. We can perform further analysis on these outliers to understand what could be driving factors for approving the loan.
5. The top 10 correlation matrix for both the datasets has further confirmed the EDA.
6. It would have been useful if the data for variables like term of loan, purpose of the loan, down payment rate, down payment amount could be tracked for current applicants as well.
