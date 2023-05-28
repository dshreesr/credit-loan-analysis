# Credit Risk Analysis
**Problem Statement:** To find the patterns, variables or driving factors in the data that will help avoid denying the loan to the applicants capable of repaying it.

**A little about Data:**
We have two types of data for analysis:
1. Current applicants - with details like what is their application status, loan credit amount, income, living situation, family status, assets they own etc.
2. Previous application data of the applicant.
3. The current applicant file has a variable Target, which takes values 0,1. 0 stands for people who have paid the loan and 1 for those you have difficulty is paying.

**Analysis Steps:**

1. All the applicants who have difficulty in paying the loan, have been grouped together in the dataframe called as defaulters and other have been grouped in dataframe called as repayers.
2. I am doing the further analysis of the dataset by comparing other variables of the dataset with these features.
3. Similarly for previous applications data we have 4 different categories based on the status of the loan – approved, cancelled, refused, unused offer.
4. For the purpose of analysis, I have used the data with Approved and Refused status and compared the other variables w.r.t to these two categories
5. The previous application file also has the details of current application ID – which helps us understand how many times the user with the current loan application has previously applied for the loan and what was his status. 
6. I have further segmented the data on this basis and tried to verify the findings derived from EDA.
7. This has helped to understand what could be the driving factors giving the capable applicant the required loan.

**Insights:**

Below are some important relationship found during the EDA. Please find the more details in the attached code.

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/d4d6481c-02c9-45d2-836a-3559ab74ff82)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/65ca55de-0d7c-424e-95d1-8e58fdbbb21a)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/4455839d-1f72-4a37-b0aa-89840954dd4c)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/39e5eee0-ec1a-44e2-af88-0b199104c0fb)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/887b0bd6-3d9e-48de-a88f-cedc5fb6f383)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/08005bd8-f2b5-4f6b-bb6d-1f2982c787b3)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/4fb9f92f-0b4b-45f6-948c-8dd74f9915db)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/258951f3-0b1c-45f3-bb07-df380f0e9bda)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/1b933784-65c6-4515-8055-3245f837991e)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/f8322f87-73f9-485a-8e11-1d3bed01696c)

![image](https://github.com/dshreesr/credit-loan-analysis/assets/33718332/ebf19fae-b2f5-4d89-9a64-db777499ad56)

**Conclusion:**
1. The current and previous application data is imbalanced. Distribution of its variables is skewed.
2. We were able to confirm few observations from the EDA.
3. We can conclude that person’s age, car and flat ownership, population density of the area in which they reside, overall living situation assessment, documents submitted - these variables could be considered as driving factors while identifying the applicants capable of repaying the loan.
4. Also in certain cases we have observed that outliers where the applicant has re-payed the loan. We can perform further analysis on these outliers to understand what could be driving factors for approving the loan.
5. The top 10 correlation matrix for both the datasets has further confirmed the EDA.
6. It would have been useful if the data for variables like term of loan, purpose of the loan, down payment rate, down payment amount could be tracked for current applicants as well.
