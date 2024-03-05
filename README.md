# PwC-Switzerland-Power-BI-in-Data-Analytics-Virtual-Case-Experience

## Task 2-Call Centre Trends
Visualizing customer and agent behavior Create a dashboard in Power BI for Call Centre Manager that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset.

### **Table of Contents:**
**• Problem Statement**

**• Flow of work-:**

Step 1- Upload Data
             
Step 2-Cleaning data
            
Step 3-Transform data
             
Step 4-Load data 

**• Data Preparation**

Data Modelling

Writing DAX 

**• Data Visualization**

**• Data Analysis**

**• Insights**

**• Shareable link**

**•Problem Statement**

The purpose of this analysis is to create a dashboard in PowerBI for call canter manager that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset. Get creative!

Possible KPIs include (but are not limited to):

• Overall customer satisfaction

• Overall calls answered/abandoned

• Calls by time

• Average speed of answer

• Agents performance quadrant -> average handle time(talk duration) vs calls answered

**• Flow of work**

**Step 1- Upload Data**

The Dataset used for this analysis was presented by PWC_Switzerland and available at their official website page - [Dataset_link]

**Step 2-Cleaning data**

Data transformation was done in Power Query and the dataset was loaded into Microsoft Power BI Desktop for modelling.The call canter dataset is given by a table named:

• Call Center which has 10 columns and 5000 rows of observation

The tabulation below shows the Call center table with its column names and their description:

| Column Name | Description |
|--- | --- |
| Call Id | Represents every unique observation in the dataset |
| Agent | Describes the name of the agent |
| Date | Describes the date of the call |
| Time | Represents the time of the call |
| Topic | Describes the topic of the caller |
| Answered | (Y/N) Describes if the call was Answered or not |
| Resolved | Describes if the problem was Resolved or not |
| Speed of answer(in seconds) |	Represents the speed of answer in seconds|
| AvgTalkDuration	| Represents the average talk duration of call |
| Satisfaction rating |	Represents the satisfaction rating of the agent during the call |

**Step 3-Transform data**

Data Cleaning and transformation for the dataset were done in power query as follows: 

• Unnecessary columns were removed 
• Each of the columns in the table was validated to have the correct data type 
• Unnecessary rows were removed


**Data Visualization**

Data visualization for the datasets was done in Microsoft Power BI Desktop: 

• The Call Center Manager Page: Shows KPIs including overall customer satisfaction, overall calls answered/abandoned, calls by time, average speed of answer, agents performance quadrant -> average handle time(talk duration) vs calls answered

**Data Analysis**

Measures used in visualization are:

• %TotalCallsAnswered = DIVIDE([CallsAnswered],COUNT('Call Center Data'[Call Id]))

• CallsAnswered = CALCULATE(COUNT('Call Center Data'[Answered (Y/N)]),'Call Center Data'[Answered (Y/N)]="Y")

• CallsMissed = CALCULATE(COUNT('Call Center Data'[Answered (Y/N)]),'Call Center Data'[Answered (Y/N)]="N")

• IssueResolved = CALCULATE(COUNT('Call Center Data'[Resolved]),'Call Center Data'[Resolved]="Y")


Insights
As shown by Data Visualization, It can be deduced that:

• The average satisfaction rating is 3.40

• 4054 calls were answered and 3646 issues resolved

• Jim has the highest satisfaction rating

• The average speed of answer is 67.52 seconds

• Jim has answered total 536 call which is highest whereas Stewart answered lowest number of calls i.e. 477


**Dashboard image**
![Call Center Trends Image](https://github.com/Sambhaji968/PwC-Switzerland-Power-BI-in-Data-Analytics-Virtual-Internship-Case-Experience/assets/157734829/97edc7ea-22ed-4543-9e92-3e101e009cce)



## **Task 3-Customer Retention-Customer demographics and insights.**

### ***Table of Contents:**

**• Problem Statement**

**• Flow of work-:**

Step 1- Upload Data
             
Step 2-Cleaning data
            
Step 3-Transform data
             
Step 4-Load data

**• Data Preparation**

Data Modelling


Writing DAX 


**• Data Visualization**

**• Data Analysis**

**• Insights**

**• Shareable link**

**•Problem Statement**

The telecom Retention Manager has scheduled a meeting with the engagement partner at PwC to cover these points:

• Customers in the telecom industry are hard-earned: we don’t want to lose them.

• The retention department is here to get customers back in case of termination.

• Currently, we get in touch after they have terminated the contract, but this is reactionary: it would be better to know in advance who is at risk.

• We have done customer analysis with Excel: it has always ended in a dead-end.

• We would like to know more about our customers: visualised clearly so that it’s self-explanatory for our management.

Your colleague, the engagement partner, asks you to do the following tasks:

1. Define proper KPIs

2. Create a dashboard for the retention manager reflecting the KPIs

3. Write a short email to him (the engagement partner) explaining your findings, and include suggestions as to what needs to be changed

Here are some inputs:

• Customers who left within the last month

• Services each customer has signed up for: phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies

• Customer account information: how long as a customer, contract, payment method, paperless billing, monthly charges, total charges and number of tickets opened in the categories administrative and technical

• Demographic info about customers – gender, age range, and if they have partners and dependents

**• Flow of work**

**Step 1- Upload Data**

The Dataset used for this analysis was presented by PWC_Switzerland and available at their official website page - [Dataset_link]

**Step 2-Cleaning data**

Data transformation was done in Power Query and the dataset was loaded into Microsoft Power BI Desktop for modelling.The Customer Retention dataset is given by a table named:

• Customer retention which has 23 columns and 7043 rows of observation

The tabulation below shows the Customer retention table with its column names and their description:

| Column Name |	Description |
| --- | --- |
| customerID  |	Represents the unique number of the customer in the dataset |
| gender  | Describes the gender of the customer | 
| SeniorCitizen  |	Describes if the customer is a senior citizen |
| Partner  |	Describes if the customer has a partner |
| Dependents  |	Describes if the customer has a dependent |
| tenure  | Describes how long as a customer |
| PhoneService  | Describes if the customer has registered a phone service |
| MultipleLines  |	Describes if the customer has registered multiple lines |
| InternetService  |	Describes if the customer has registered for internet service |
| OnlineSecurity  |	Describes if the customer has registered for online security |
| OnlineBackup  |	Describes if the customer has registered for online backup |
| DeviceProtection  |	Describes if the customer has registered for device protection |
| TechSupport  |	Describes if the customer has registered for tech support |
| StreamingTV  |	Describes if the customer has registered to stream tv |
| StreamingMovies  |	Describes if the customer has registered to stream movies |
| Contract  |	Describes if the length of the contract of the customer |
| PaperlessBilling  |	Describes if the customer has registered for paperless billing |
| PaymentMethod  |	Describes the payment method of the customer |
| MonthlyCharges  |	Represents the monthly charge incurred by the customer |
| TotalCharges  |	Represents the total charge incurred by the customer |
| numAdminTickets  |	Represents the number of admin tickets opened by the customer |
| numTechTickets  |	Represents the number of tech tickets opened by the customer |
| Churn  |	Describes if the customer is at risk of churn |


**Step 3-Transform data**

Data Cleaning and transformation for the dataset were done in power query as follows: • Each of the columns in the table was validated to have the correct data type • Unnecessary rows were removed

**Data preparation: -**

**Data Modelling**

After the dataset was cleaned and transformed, it was ready to be modelled. • The official dataset is marked as the 01 CHURN-Dataset table in the dataset.

• Along with this, a separate table- All Measuress is created to store all the measures which we have used in this model.

**Data Visualization**

Data visualization for the datasets was done in Microsoft Power BI Desktop:

• Demographic Info : Shows the male-female distribution,churn by senior citizen,dependents impact,partner impact effect of internet service provider recommendations and a short insight on the report

• Account Info : shows contrct type payment method tenuraity impact on customer count total charges, average monthly charges etc

• Services : shows customer count by streamingTV,customer count by streamingmovies,churn by phoneservice,online security device protection,Tech support etc

• Email / Insights and suggestion :Insights ans suggestions to the engagement partner explaining findings, and include suggestions as to what needs to be changed

**Data Analysis**

Measures used in visualization are:

• Average MonthlyCharges = AVERAGE('01 Churn-Dataset'[MonthlyCharges])

• Average TotalCharges = AVERAGE('01 Churn-Dataset'[TotalCharges])

• churn count = CALCULATE(COUNT('01 Churn-Dataset'[Churn]), ALLSELECTED('01 Churn-Dataset'[Churn]),'01 Churn-Dataset'[Churn] = "yes")

• churn rate % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[Churn]), '01 Churn-Dataset'[Churn] = "yes" ), COUNT('01 Churn-Dataset'[Churn]), 0)

• Dependent in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[Dependents]), '01 Churn-Dataset'[Dependents]="Yes",'01 Churn-Dataset'[Churn]="Yes"), CALCULATE(COUNT('01 Churn-Dataset'[Dependents]),'01 Churn-Dataset'[Churn]="Yes"), 0)

• Device protection in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[DeviceProtection]), '01 Churn-Dataset'[DeviceProtection] ="Yes", '01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[DeviceProtection]),'01 Churn-Dataset'[Churn]="Yes"),0)

• loyalty = SWITCH(TRUE(),'01 Churn-Dataset'[tenure]<=12,"< 1 year",'01 Churn-Dataset'[tenure]<=24,"< 2 years",'01 Churn-Dataset'[tenure]<=36,"< 3 years",'01 Churn-Dataset'[tenure]<=48,"< 4 years", '01 Churn-Dataset'[tenure]<=60,"< 5 years",'01 Churn-Dataset'[tenure]<=72,"< 6 years")

• Online backup in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[OnlineBackup]), '01 Churn-Dataset'[OnlineBackup] ="Yes", '01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[OnlineBackup]),'01 Churn-Dataset'[Churn]="Yes"),0)

• Online security in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[OnlineSecurity]), '01 Churn-Dataset'[OnlineSecurity] ="Yes", '01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[OnlineSecurity]),'01 Churn-Dataset'[Churn]="Yes"),0)

• Partner in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[Partner]),'01 Churn-Dataset'[Partner]="Yes",'01 Churn-Dataset'[Churn]="Yes"), CALCULATE(COUNT('01 Churn-Dataset'[Partner]), '01 Churn-Dataset'[Churn]="Yes"), 0)

• Phone service in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[PhoneService]), '01 Churn-Dataset'[PhoneService] ="Yes", '01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[PhoneService]),'01 Churn-Dataset'[Churn]="Yes"),0)

• SenioCitizen in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[SeniorCitizenChurn]),'01 Churn-Dataset'[SeniorCitizenChurn]=1,'01 Churn-Dataset'[Churn]="Yes"), CALCULATE(COUNT('01 Churn-Dataset'[SeniorCitizenChurn]),'01 Churn-Dataset'[Churn]="Yes"), 0)

• SeniorCitizen = SWITCH('01 Churn-Dataset'[SeniorCitizenChurn],0,"No",1,"Yes")

• Streaming Movies in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[StreamingMovies]), '01 Churn-Dataset'[StreamingMovies] ="Yes", '01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[StreamingMovies]),'01 Churn-Dataset'[Churn]="Yes"),0)

• Streaming TV in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[StreamingTV]), '01 Churn-Dataset'[StreamingTV] ="Yes", '01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[StreamingTV]),'01 Churn-Dataset'[Churn]="Yes"),0)

• Tech Support in % = DIVIDE(CALCULATE(COUNT('01 Churn-Dataset'[TechSupport]), '01 Churn-Dataset'[TechSupport] ="Yes", '01 Churn-Dataset'[Churn]="Yes"),CALCULATE(COUNT('01 Churn-Dataset'[TechSupport]),'01 Churn-Dataset'[Churn]="Yes"),0)


**Insights**

As shown by Data Visualization, It can be deduced that:


• Higher churn rate:

Younger customers (under 3 years).

Customers paying by check or bank transfer. 

Customers with paperless billing.

Customers with monthly subscriptions.


• Lower churn rate:

Customers with senior citizen discount.

Customers with multiple lines of service.

Customers with annual subscriptions.

Customers with automatic payments.

• If no Tech Support, Device Protection, and Online Security are provided then the chances of customers churning are high.

• payment method like Electronic check also makes a significant impact on the churning decision.

• There is no relation between gender with churning.

• senior citizens are less likely to churn rate.

• Customers with any dependents or partners are churning less likely, whereas the non-dependents and non-partners customers are more likely to shift.

• Tenure and contract play an important role in determining whether the customer will churn. Customers with monthly contracts i.e. lower tenure will switch frequently.

• Customers with Fiber Optic internet service will churn more compared to DSL internet service holders.

**Suggestions**

• Increasing the basic contract plan from 1 month to 3 months or 6 months can be a good starting point. This will help customers to be with us for a longer tenure.

• Starting special offers or schemes for customers who are single and have no family responsibility. They can become a permanent customer of the company. 'Catch them Young' is key to success here.

• provide some offers to the senior citizens as they are stable customers like overall offer some discounts on long tenure plans.

• Offering basic services like device protection, tech support, and online security should be the primary goal. This will help the customer stay longer with the brand.


**Dashboard image**

**Figure 1. shows visualizations from Customer churn Exploratory)**
![Customer churn Exploratory Dashboard  image](https://github.com/Sambhaji968/PwC-Switzerland-Power-BI-in-Data-Analytics-Virtual-Internship-Case-Experience/assets/157734829/7ac5ea16-a426-4416-aa42-d0e7a77714fb)


**Figure 2. shows visualizations from Customer Risk Analysis**
![Customer Risk Analysis Image](https://github.com/Sambhaji968/PwC-Switzerland-Power-BI-in-Data-Analytics-Virtual-Internship-Case-Experience/assets/157734829/fb10bf60-b6f8-48f4-bbac-c60756a34c01)


