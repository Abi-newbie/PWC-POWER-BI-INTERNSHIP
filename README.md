# PWC-POWER-BI-INTERNSHIP

PWC has designd a Digital Accelerator programme on Forage and its an internal chance that takes groups of employees out of their day jobs and puts them through  trainings that teaches them skills in technology such as automation, machine learning, design thinking, and digital storytelling. PowerBI is an important part of it as visualising data helps to handle and understand clients. As a digital Accelarator I have being tasked by companies to help solve issues relating to their call centre, customers churns and diversity and inclusion.


#  Task 1 Call Centre KPI

It’s omnipresent: telecom marketing. Better price here. Better service there. Best for small businesses here. Best for young urbanites there. But what do customers really want? Our client, a big telecom company needs to know. Phone now has tasked me to perform the underlisted task

# TASK

Create a dashboard in Power BI for visualizing relevant KPIs and metrics in the dataset provided
Respond to the client's request by providing a well-designed Power BI dashboard reflecting the requested KPIs.
Overall customer satisfaction
Overall calls answered/abandoned
Calls by time
Average speed of answer
Agent’s performance quadrant -> average handle time (talk duration) vs calls answered

# Measures used


# Answered calls= Calculate(Count(Sheet1 [Callid]),Filter(Sheet1,Sheet1(Answered(Y/N)="Y"))

# Calls Not Answered = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Answered (Y/N)]="N"))

# Not Resolved = CALCULATE(COUNT(Sheet1[Topic]),FILTER(Sheet1,Sheet1[Resolved]="N"))

# Resolved Calls = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Resolved]="Y"))

# Total = COUNT(Sheet1[Call ID]

DATA VISUALIZATION

![Screenshot (12)](https://github.com/user-attachments/assets/ce88574c-b95f-4386-a40a-dbe07bf96132)


#  INSIGHTS

This findings shows that the total numberof calls that came through was 5000
Average speed for answering calls was 67.52
the top ten agents did not have ratings of 4 or above
calls not resolved summed up to 946
the overall call satisfaction rating was 3.40
81% of calls were answered while 72.92% of the call related issues were resolved

# Recommendations


Agents must be educated and trained on the impotance and power of ratings and how it affects the company
Calls must be answered promptly to reduce the number of unanswered calls
Agents should be well trained nd equipped in order to be in the postion to resolved all issues


# TASK 2 : CUSTOMER CHURN

Create a dashboard using the defined KPIs to reflect customer demographics and insights.
Write a concise email to the engagement partner explaining your findings and providing suggestions for necessary changes based on the dashboard you've created.
Define key performance indicators (KPIs) related to customer retention.
Create a dashboard that visualizes customer demographics and insights.

# INFORMATION ON TASK

Customers in the telecom industry are hard-earned: we don’t want to lose them
The retention department is here to get customers back in case of termination 
Currently, we get in touch after they have terminated the contract, but this is reactionary: it would be better to know in advance who is at risk 
We  have done customer analysis with Excel: it has always ended in a dead-end
We would like to know more about our customers: visualised clearly so that it’s self-explanatory for our management

# MEASURES

# Average MonthlyCharges = AVERAGE('01 Churn-Dataset'[MonthlyCharges])

# Average TotalCharges = AVERAGE('01 Churn-Dataset'[TotalCharges])

# Churn Rate% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[Churn]),'01 Churn-Dataset'[Churn]="yes"),COUNT('01 Churn-Dataset'[Churn]),0)

# Customer Churn = CALCULATE(COUNT('01 Churn-Dataset'[Churn]),ALLSELECTED('01 Churn-Dataset'[Churn]),'01 Churn-Dataset'[Churn]="Yes")

# Dependent in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[Dependents]),'01 Churn-Dataset'[Dependents]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[Dependents]),'01 Churn-Dataset'[Churn]="Yes"),0)

# Device Protection in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[DeviceProtection]),'01 Churn-Dataset'[DeviceProtection]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[DeviceProtection]),'01 Churn-Dataset'[Churn]="Yes"),0)

# Online backup in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[OnlineBackup]),'01 Churn-Dataset'[OnlineBackup]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[OnlineBackup]),'01 Churn-Dataset'[Churn]="Yes"),0)

# Online Security in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[OnlineSecurity]),'01 Churn-Dataset'[OnlineSecurity]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[OnlineSecurity]),'01 Churn-Dataset'[Churn]="Yes"),0)

# Partner in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[Partner]),'01 Churn-Dataset'[Partner]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[Partner]),'01 Churn-Dataset'[Churn]="Yes"),0) 

# Phone Service in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[PhoneService]),'01 Churn-Dataset'[PhoneService]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[PhoneService]),'01 Churn-Dataset'[Churn]="Yes"),0)

# Senior Citizens in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[SeniorCitizen]),'01 Churn-Dataset'[SeniorCitizen]=1,'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[SeniorCitizen]),'01 Churn-Dataset'[Churn]="Yes"), 0)

# Streaming Movies in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[StreamingMovies]),'01 Churn-Dataset'[StreamingMovies]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[StreamingMovies]),'01 Churn-Dataset'[Churn]="Yes"),0)

# Streaming Tv in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[StreamingTV]),'01 Churn-Dataset'[StreamingTV]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[StreamingTV]),'01 Churn-Dataset'[Churn]="Yes"),0)

# Tech support in% = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[TechSupport]),'01 Churn-Dataset'[TechSupport]="Yes",'01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[TechSupport]),'01 Churn-Dataset'[Churn]="Yes"),0) 

# Total Customer Churn = COUNT('01 Churn-Dataset'[customerID])


# FINDINGS


Findings indicates that customers signed on to the two years contract have been with the company for a long time while new clients are opt for the month-to-month contracts. 
 
From the analysis the company is at risk at loosing new clients if they sign on month-to-month contract. Total churning rate is at 27% which indicates that 7043 customers are at risk of churn.

2173 tech tickets were raised by churned customers while 885 Admin tickets were opened.  It is observed that customers who churned did not sign up for device protection, online back up and security and tech support.

0.42 customers who churned were using fire optic as their internet service providers.

 # RECOMMENDATIONS

The company should advertise the benefits of subscribing to the one- two years contracts since the payment is not monthly based as compared to month-to-month contract. 
 
Customers should be educated on the importance of signing up for services such as online backup and security, tech support and device protection.
Sales and discounts on some products and services plays an important role in attracting and retaining customers. Hence these must be introduced periodically. 

# DATA VISUALISATION

![image](https://github.com/user-attachments/assets/aac81f75-138c-4065-81e5-9a0e657aded3)

![image](https://github.com/user-attachments/assets/ec7b855b-42f2-4287-a446-48d8ef530a0e)

![image](https://github.com/user-attachments/assets/f580d0b5-cb75-4d1d-82b6-652e8f391dc1)


# TASK 3: DIVERSITY AND INCUSION

# TASK

Define relevant KPIs in hiring, promotion, performance and turnover, and create a visualisation

Write what you think some root causes of their slow progress might be

Create visualizations to represent HR data, particularly focusing on gender-related KPIs.

Identify and discuss potential root causes for the slow progress in achieving gender balance at the executive management level.

Define key performance indicators (KPIs) related to gender balance and diversity.

Create visualizations that represent HR data effectively.

The imperatives of diversity and inclusion in the corporate world.

# BACKGROUND INFORMATION

Human Resources at our telecom client is highly into diversity and inclusion. They’ve been working hard to improve gender balance at the executive management level, but they’re not seeing any progress. They’re reaching out to us for help.

At PwC Switzerland we are often approached by clients seeking support with diversity and inclusion. Companies need a workforce of diverse talents and backgrounds to succeed in an increasingly complex and heterogeneous world. To us, diversity and inclusion are business imperatives, not just nice-to-haves. We aim for all of our teams to feel welcome and appreciated. But actually achieving this and unlocking its potential involves a whole set of practical challenges

# MEASURES

# #Female Hire = CALCULATE(DISTINCTCOUNT('Pharma Group AG'[Employee ID]),FILTER('Pharma Group AG','Pharma Group AG'[Gender]="Female"))

# #Male Hire = CALCULATE(DISTINCTCOUNT('Pharma Group AG'[Employee ID]),FILTER('Pharma Group AG','Pharma Group AG'[Gender]="Male"))

# #Not Promoted = CALCULATE(DISTINCTCOUNT('Pharma Group AG'[Employee ID]),FILTER('Pharma Group AG','Pharma Group AG'[Promotion in FY21?]="No"))

# #of Leavers = CALCULATE(DISTINCTCOUNT('Pharma Group AG'[Employee ID]),FILTER('Pharma Group AG','Pharma Group AG'[FY20 leaver?]="Yes"))

# #of Total Hire = (COUNT('Pharma Group AG'[Employee ID]))

# #of Turnover = CALCULATE(COUNT('Pharma Group AG'[Employee ID]),FILTER('Pharma Group AG','Pharma Group AG'[In base group for turnover FY20]="Y"))

# #of Turnover by Females = CALCULATE(COUNT('Pharma Group AG'[In base group for turnover FY20]),'Pharma Group AG'[In base group for turnover FY20]="Y",'Pharma Group AG'[Gender]="Female")

# #of Turnover by Male = CALCULATE(COUNT('Pharma Group AG'[In base group for turnover FY20]),'Pharma Group AG'[In base group for turnover FY20]="Y",'Pharma Group AG'[Gender]="Male")

# #Promoted = CALCULATE(DISTINCTCOUNT('Pharma Group AG'[Employee ID]),FILTER('Pharma Group AG','Pharma Group AG'[Promotion in FY21?]="Yes"))

# % of Female = DIVIDE('Pharma Group AG'[# Female Hire],'Pharma Group AG'[# Female Hire]+'Pharma Group AG'[# Male Hire])

# % of Male = DIVIDE('Pharma Group AG'[# Male Hire],'Pharma Group AG'[# Male Hire]+'Pharma Group AG'[# Female Hire])

# % of Male Promoted = DIVIDE('Pharma Group AG'[# Male Hire],'Pharma Group AG'[# Promoted])

# % of Turnover = DIVIDE('Pharma Group AG'[# of Turnover by Females],'Pharma Group AG'[# of Turnover by Male]+'Pharma Group AG'[# of Turnover])

# % of Women Promoted = DIVIDE('Pharma Group AG'[# Female Hire],'Pharma Group AG'[# Promoted])

# % Promoted = DIVIDE('Pharma Group AG'[# Promoted],'Pharma Group AG'[# Promoted]+'Pharma Group AG'[# Not Promoted])

# Avg Men Rating = CALCULATE(AVERAGE('Pharma Group AG'[FY20 Performance Rating]),FILTER('Pharma Group AG','Pharma Group AG'[Gender]="Male"))

# Avg Women Rating = CALCULATE(AVERAGE('Pharma Group AG'[FY20 Performance Rating]),FILTER('Pharma Group AG','Pharma Group AG'[Gender]="Female"))
% of Turnover = DIVIDE('Pharma Group AG'[# of Turnover by Females],'Pharma Group AG'[# of Turnover by Male]+'Pharma Group AG'[# of Turnover])


# DATA VISUALIZATION

![image](https://github.com/user-attachments/assets/bbace4fc-517e-413f-895d-a6df38688e1a)

![image](https://github.com/user-attachments/assets/ed59ff0b-8d0c-4c4b-aea8-b3b44ee8f4f1)

![image](https://github.com/user-attachments/assets/2e4f0c53-4bac-4ebf-ae3b-98ca7f108035)


# INSIGHTS

There seem to be a great difference in hiring and promotion between genders. There is gender imbalance and bais as more men are being hired(59%) and promoted(5.78) in the Manager, Senior Manager, Director and executive positions while females are more promoted and hired  in the junior level than in senior position. pecentage of female hired(41) and percentage promoted is promoted(4.02).

Turnover rate for men is 263 while total nmber of turnover for female is 171. More males who leave belong to the senior job level while majority of females who leave belong to the junior job levels. Employees belonging the to 20-39 age group leave the most.

Total number of employees hired is 500 with 205 being females and 295 being males. The average rating for men is 2.41 while that of female is 2.42 this rating does not correlate to the number of male and females hired inthe company.


# RECOMMENDATIONS

Employers mut take necessary steps to eliminate bias in hiring and prmotion stage if any exist
There should be equal oppotunities created this can be creating career groeth opportunitis for females promote diversity and promote healthy environment.
survey should be sent to employes on ways to increase rention 

# TECH STACK

MICROSOFT EXCEL

POWER BI

DAX

POWER QUERY































