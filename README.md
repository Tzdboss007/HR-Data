# HR-Data-Documentation
![](HR.JPG)
- These are the comprehensive documentation of the HR data which contains information on staff in an organization.

---
## Project Overview
The HR Data is a record of a survey taken by staff members in an organization, this data consists of staff age range, staff Attrition, department, job level, job satisfaction, monthly income, and educational level to mention a few. 
In this project, I seek to know the root cause of the high attrition rate, the factors contributing to the attrition rate, and the correlation between attrition and some other factors that may be influencing the exit of staff in the company.
 
---
## Project Outline
- HR-Data-Documentation [HR Data Documentation](#hr-data-documentation)
- Project Overview [Project Overview](#project-overview)
- Data Source [Data Source](#data-source)
- Tools Used  [Tools Used](#tools-used)
- Data cleaning [Data cleaning](#data-cleaning)
- Data Analysis [Data Analysis](#data-analysis)
- Findings And Conclusion [Findings And Conclusion](#findings-and-conclusion)

---

## Data Source 
The source of the HR data used in this Analysis is from skilhavest practical class  [ClICK HERE TO DOWNLOAD](https://tinyurl.com/2udjsy98) 

---

## Tools Used 
 tool used for both the Analysis and Visualization of the above data Includes 
- PowerBI
- Power Query
- Google sheet [click Here To View](https://tinyurl.com/2udjsy98)
---
## Data cleaning 
In a bid to clean the data for onward use, some basic operations were carried out on the data before use

- Promotion of row header: The first roll was promoted to make up for the header which was not indicated in the raw data
- Change data type: The data types of some certain columns were changed from the default string values to Numbers
- Addition of conditional columns: To effectively sort the age range column in chronological order during the analysis a
  conditional column was created. 
---
## Data Analysis
The data used in this analysis has been partially cleaned, in my analysis I tried to first find the total number of employees in the company then I proceeded to get the number of retained staff, I was also able to get the attrition count then from the attrition count and number of employee i calculated the rate of attrition in the organization and also find the average age of an employee in the organization. 

The number of retained staff was calculated using the DAX function
```
Retained Staff = sum('HR data'[Employee Count])-sum('HR data'[Attrition Count])
```
The rate of attrition was calculated using the DAX function 
```
Attrition Rate = sum('HR data'[Attrition Count])/sum('HR data'[Employee Count])
```
- I tried to check for job satisfaction by job role and attrition count by department
- I also tried to see the correlation between attrition by education and marital status
- I tried to see the relationship between attrition, education, and gender 
- And the relationship between attrition, age band, and Gender
---

Findings And Conclusion
The dashboard below shows the results of the analysis carried out on the HR data. From  the dashboard, we have a total of 1470 total employees and 1233 retained employees. Also, we have a total of 237 attrition which accounted for the 16% attrition rate and an average age of 37 years.
The following was deduced from the analysis as shown on the dashboard using a pie chart the attrition count by the department the R&D department with 133 employees attrition and the sales department coming second with 92 employees while the HR has the least number with just 12 employees.

![](HR1.JPG)

![](HR2.JPG)
