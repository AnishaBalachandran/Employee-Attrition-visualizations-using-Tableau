CHAPTER 1: INTRODUCTION 
In this report, various aspects of HR Metrics for a large pharmaceutical company will be analysed, mainly focusing on their high employee attrition rate problem, through data visualizations using Tableau, for the better understanding of the business problem by the HR Managers and other potential business users. Recently, there has been increased focus on workforce analytics in helping HR professional and business partners (Kryscynski el al., 2017). Few of the challenges faced in transition to data driven analytics from traditional analytics include usage of irrelevant metrics, usage of simple measures, ignorance of non-quantitative measures etc (Davenport et al., 2010). In this study, Descriptive Analytics and Diagnostics Analytics is implemented using tools and techniques like visualization, data discovery, drill-down and data mining methods to get insights into the business problem. (Gupta and Sharma, 2023). 

CHAPTER 2: METHODOLOGY
2.1. Data Source and Method
The pharmaceutical company 1 year data extracted from their HR Information system, in excel with 35 variables and 1467 observations was used. Tableau Prep Builder2023.3 was used for prepping of data for data quality issues and Tableau 2023.2 was used for data visualization and dashboard preparation
2.2. Overview of steps Undertaken
![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/61f52f7e-0110-41b6-8414-ba3167e23055)
2.3. Quality Assessment
As per the data analysis of the data 1467 observations, 3 data quality issues were identified. Data Quality issues were addressed using Tableau Prep Builder.
1.	Department variable had values “HR”, “Human Resources”,” R&D”, “Research & Development” and “Sales. “HR” and “Human Resources” as well as “R&D” and “Research & Development “are redundant values. Hence all “HR” values have been replaced with “Human Resources” and all “R&D” values has been replaced with “Research & Development in the considered data set using Group function.
2.	Age variable had 2 observations with values greater than 65 and 1 observation with value less than 18. These are the outliers and probably not valid in the context. Hence these 3 observations have been excluded in the considered data set using Filter function.
3.	Total Working Years variable had 1 observation with value 94, which is an outlier and probably not valid in the context. Hence this 1 observation has been excluded in the considered data set using Filter function.
After the data quality rectification, the output data set consists of 1463 observations.  Since these 4 observations, makes upto only 0.27% of the total data set, exclusion of these 4 observations will not have a major impact on the overall data quality.
The output dataset of 1463 observations were exported to Tableau for data visualization and dash boarding.
2.4. Creation of Calculated Fields 
4 Calculated fields generated as below
1) Leaving Employees- Assigned numerical values of 1 and 0 assigned based on the Attrition value Yes or No, using IF function
![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/6d37ce3e-2432-4566-b519-9f1808e423d0)
2)Active Employees – Calculated from total count of Employees and Leaving employees
![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/574e9251-bd61-4986-b76e-21b46d5e79ef)
3)Attrition Rate- Calculated from total count of employees and Leaving employees
![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/15fbe8e5-d3d1-4a2b-ada4-ad39062662c8)
4)Annual Billing Rate- Calculated from Monthly rate
![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/0a74abe9-058f-4a28-befd-2ab56550ea4e)
2.5. Selection of variables 
Dimensions or measures were chosen considering which can be more insights to the attrition rate of the company, mainly. Both categorical and numerical variables like age, gender, education, salary, tenure etc are considered, which give information across a people management activity (Edwards and Edwards, 2017) Out of 35 variables from the data source, 13 variables were used in the visualizations
![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/68a9d818-94d4-4f5c-82f3-3ed7f48baef1)
![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/983c3118-47d9-47bd-a25d-9204008ca9e4)
2.6. Building of Data Visualizations
A superior data visualization design strategies for narrative visualization as storytelling and visual expressions indispensable part of human culture (Segel and Heer, 2010)   The below 10 visualizations were built based on selected variables. 
1)  Major KPI s were identified with respect to the Business Problem. 

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/6e12a7b9-5004-48fb-acb6-cd01ebdd7601)
2)  Gender Wise Attrition 

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/c089cc98-c396-4ea9-88b6-6c7e3d46fc6f)
3)  Marital status and Gender Wise Attrition

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/059ab696-9fa1-4816-b1aa-f66e04547115
4)  Department wise Attrition

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/4992acbe-2da4-4909-8629-ed47bb24e573)
5) Job Role wise Attrition. Job Level has been used a filter for this visualization	

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/f285b4a5-d240-4ca8-bc42-e5df9d642ec4)
6) Education level and Education Field Wise Attrition

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/cc3fd306-70e6-4edd-8b31-18766f5f992d)
7) Age wise attrition. Age Bins are created for the range 18-32, 33-48 and 49-65. It is compared against Reference Line representing Average Attrition Rate.

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/f4f7eb40-25ec-4da1-9f96-c477734a75cc)
8)  Business Travel Frequency Wise Attrition

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/de0caf81-b205-4258-a0c1-4f99c12a6385)
9) Promotion frequency for the employees of each department in each job role 

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/a7ce37c3-2597-4f29-8f09-9a3801aaedbe)
10) Total Cost the company incurs for each job role in each department

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/8823b56a-7cf2-4d68-a3bc-9561df2b5455)
2.7. Dashboard creation
All the 10 visualizations along with2 global filters dashboard – Gender and Department. are incorporated into a dashboard for giving meaningful and interactive insights. The dashboard creation was based on 5 principles of data visualization – truthful, functional, beautiful, insightful and enlightening (Cairo, 2016).

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/0d32cd0a-b09f-4ef9-90ae-4d99e9eb4f91)



![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/d185c121-c4e2-42f4-a3f3-9f6adfb4d67a)

CHAPTER 3: FINDINGS 

The following insights were observed from these visualizations.
1) KPIs
KPIs were displayed in text tables to give a synoptic view of the of the business problem, before delving into the details. Calculated fields incorporated as shown in Figure 2, Figure 3 and Figure 4.

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/3908e14e-b7c4-479b-89ff-78d811031b5c)
This visualization shows a clear picture of the attrition rate and no of employees left during the last 1 year. It also shows the average period for which an employee stays with the company.

2) Gender wise attrition
Attrition rate analysed on basis of gender using bar chart. Further the global filter Department can be used to gender wise attrition rate for each department. 

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/1a80935c-a1c7-4f28-aaaf-ca5df5e3cb9b)
While the overall attrition among men and women is almost same, when analysed with each department a high percentage of women resign in HR department as compared to Men. Overall female attrition is less as compared to men, however more female employees resign from HR and Sales as compared to their male counterparts. 
3)  Marital status and Gender Wise Attrition
Attrition rate in line with marital status and gender is analysed using tree map as more than dimension is considered in the visualization. Th colour represents the gender and size represents the attrition rate. Department filter is used as global filter for getting further insights based on each department

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/b227bef1-e52d-4385-b312-ccfa8826d673)

The overall attrition is highest among the Single Male and Female, second highest among Married Male and Female and least among Divorced Male and Female. When compared in detail using department filter, one interesting variation in the trend found is in HR department, none of the single females resigned, however department had the highest attrition rate for divorced female.

4)  Department wise Attrition
Analysis made as per the department using pie chart, as it is single dimension. Gender is given as global filter, however the findings using global filter is same the Table 7 

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/772c042a-33e4-4f2e-ae7e-e58329973a34)
As per the visualization the highest attrition is in the Sales department and the least is in the Research Development.

5) Job Role wise Attrition 
Bar chart has been utilized for analysing attrition based on job role and job role belonging to separate department has been coloured differently for easy identification Job level has been used as filter for further insights. Further the global filter department and gender can be utilized for customized insights. Attrition rate as per the visualization in descending order is as below

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/a78d2660-782b-4ec8-a8f4-a3e9b17ec606)
The highest attrition is among the Sales Representative and the second highest is among Sale Sales Executives belonging to the Sales Department. Further on filtering with Job level, this trend continues. A variation to this is observed in Job level 5, where highest attrition is among Manager Sales. In Job level 3, all 3 departments have job roles – Sales Executive, Human Resources and Laboratory Technician, with almost similar attrition rate of 35%, 33% and 33% respectively.

6) Education level and Education Field Wise Attrition
Attrition rate based on Education field and Education level has been depicted using highlight tables as there are 2 dimensions with interconnection. The highest attrition levels are marked in pink colour in table with highest in Education level 5 - Technical Degree. Marketing field is having the overall highest attrition of 32% and Education level 1 is having the highest attrition rate of 22%. Note the overall attrition rate is 19% in the table is which is agreement with the KPIs mentioned in Figure 6.
7) Age Wise Attrition
Bins were created for age groups 18-32, 33-48 and 49-65 . Reference line of Average attrition rate is plotted using dotted lines Age wise attrition has been illustrated using histogram and the variable is a continuous numerical variable.

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/53963722-78db-42e8-bf91-19d749e186d1)
The highest attrition is among 18-32 age group. The visualization also depicts a reference line for Average Attrition Rate of 19%. While 18-32 age group is having attrition above the average attrition rate, other two groups are having attrition below the average rate. Global filter available or customized view.

8)  Business Travel Frequency Wise Attrition
Attrition Rate based on Business Travel Frequency has been depicted using packed bubbles as frequency of travel was shown in reference with the department, where colour represents the department and the size represents the attrition rate. The highest attrition in all departments is among those employees who travel frequently. Global filter available or customized view.

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/c86705b9-6651-44d1-a230-9f3b9bb4e4dc)
9) Promotion frequency for the employees of each department in each job role 
Insights on Job level wise promotion frequency has been analysed for each of the department, using side by side bars, to show job roles for each department separately. The general trend is as the job level increased the promotion frequency decreases. Global filters are available for customized view.

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/3616e7c5-3d51-4226-8f78-c041328a717a)
10) Total Cost the company incurs for each job role in each department
Total Cost incurred by the company for each job role has been depicted using Tree maps, where each box represents the role, colour represents the department and size of the box represents the average of the billing cost incurred for that particular role. Manager R&D incurs the highest cost to the company and HR incurs the least cost to the company. Calculated field incorporated as shown in Figure 5. Average function is used for getting Avg Annual Billing Rate. Global filters are available for customized view.

![image](https://github.com/AnishaBalachandran/Employee-Attrition-visualizations-using-Tableau/assets/159025182/696f68d3-35df-4d7f-b0e9-9ba7198ece1d)
11) The visualizations are arranged row wise as 1-3-3-3 segmentation in dashboard focusing on attrition rate. The dashboard gives interactive insights to the various aspects of attrition rate in the company, company cost and employee promotion. Global filters implemented as single value dropdown on the top right corner improves the interactivity with the audience.

CHAPTER 4: RECOMMENDATIONS AND DISCUSSIONS
4.1. Recommendations for reducing attrition
Factors affecting attrition can be broadly classified as – work related, employer related, compensation related and employee skill set related (Adhikari, 2009). Efficient people management skills greatly reduce the employee attrition in a company (Hoffman and Tadelis, 2021) reduce the Based on the data visualization analysis, the following recommendations may be considered for reduction in attrition rate in the company.
1)	A department specific employee survey may be conducted for Sales department, to get to the root cause of the churn rate in the department. 
2)	HR department need to analyse the specific reason for high attrition in divorced female in the department, which is standing out adversely as compared to the general trend in the company.
3)	Fostering a sense of belonging in young employees in age group 18-32 , from the start through effective onboarding ensures that understand and connect with the company culture.
4)	Single employees leaving the company can be reduced to an extent by providing incentives and fast career promotions based on talent.
5)	More focus is to be given on retention of Job level 3 employees, as the attrition rate is high among them.  This trend continuing can be very adverse for the company, as this group is the people with ample experience and still very young who can contribute immensely to the company.
6)	Business Travelling may be kept to a minimum and virtual options may be explored. High travel frequency is causing some dissatisfaction among the employees across the departments. Reducing the travel frequency may increase the employee satisfaction and reduce the company cost, giving dual benefit.

4.2. Recommendations for follow up work
Human Resources must evolve into a strategic collaborator by offering insights through data analytics, enabling the formulation of competitive strategies; failure to do so risks losing relevance (Vargas et al., 2018).  Descriptive analytics of the HR metrics was successfully done using Tableau in this study.  
Further the analytics purview can be enhanced using predictive and prescriptive analytics, using regression analysis, machine learning and neural networks for forecasting and optimization of system performance (Watson, 2013). Data mining for advanced analytics can be performed using IBM Watson and R studio. (Mishu, 2018).




















