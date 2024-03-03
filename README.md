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





