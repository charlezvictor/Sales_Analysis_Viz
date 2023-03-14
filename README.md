# Sales-Analysis-Viz
 
![Sales Analysis Dashboard.png](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Sales%20Analysis%20Dashboard.png)

### Power BI Visualization Reporting Sales Analysis over time
---

## INTRODUCTION
A power BI project on sales analysis carried out to derive insights from previous year sales in order to make data driven decisions.

**_Disclaimer_**: _All datasets and reports do not represent any company, but just a dummy dataset to showcase several functionalities of Power BI._ 
Dataset can be found [here](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Budget%20and%20Sales%20Data.xlsx)


## PROBLEM STATEMENT 
1.	Sales growth from year to year?
2.	How has revenue performed from year to year?
3.	Variance between budgeted sales and current sales?
4.	Current Sales increase per year and forecast in the next one year?
5.	Which product is performing well in the market?


## SKILLS / CONCEPT DEMONSTRATED
The following Power BI concepts were put in place
-	DAX
-	Quick measures
-	Data Modelling
-	Tooltips


## MODELLING
Power BI as it would usually do, automatically derived a relationship between tables which were accurate, but I needed to create another table to aid my analysis and thus appended the Data model to create a preferred Model, then from the model, I hid certain columns that wouldn’t be necessary during analysis and report generating


Adjusted Model                  |       Preferred Model          |        Auto-Model                   
:------------------------------:|:------------------------------:|:--------------------:
![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(510).png) | ![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(511).png) | ![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(506).png)


## VISUALIZATION

![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Dashboard_Screenshot.png)
---

#### Features
 KPI showing
-	Revenue generated from current year sales
-	Revenue generated from previous year sales
-	Budgeted revenue 
-	% of Budget Variance
-	%YOY sales growth
Current year sales by Product Category
Monthly Trend of Sales
YOY sales Growth% and Current Sales by product name
Current sales trend by year

### Downlaod PowerBI report [here](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Sales%20Analysis%20Dashboard.pbix) and interact with it 

You can downlaod a Pdf version of the report [here](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Sales%20Analysis%20Dashboard.pdf)

## KEY PROCESS INVOLVED
For the sake of documentation I woul go through a step by stwp process of how certain mesaures were created that aided in developing this dashboard.

##### 1. A new table name **Date Dim** short for Date Dimension was created, and this was cretaed to extracted the date from the tables using the _**CALENDERAUTO()_** function. Then the Quarter and month column was created.
 Picture is shown below
 
DATE DIM TABLE WITH CALENDERAUTO FUNCTION   |       EXTRACTED YEAR AND MONTH                  
:------------------------------------------:|:-------------------------------:
![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(508).png) | ![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(509).png)

#### 2. Created the **Current Year**, CY measure whereby I used the lastest year in the Date Dim table by selecting the _Maximum_ Function, the calculated the total sum of sales fro that year using the _Calculate and Sum Function_



![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(515).png)


#### 3. Created the **Previous Year** , PY measure by refrencing the CY Sales meaure **AND** _THESAMEPERIODLASTYEAR_ from the Date Dim Table


![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(516).png)

#### 4. Created the **Budgeted Sales** measure by repeating the steps in created CY measure but changing _'Sales Amount'_ to _'Budgeted Amt'_


![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(513).png)

#### 5. **YOY Sales Growth** and **Budgeted Varince** the same way, just basic maths:


YOY SALES GROWTH                   |       BUDGETED VARIANCE                  
:---------------------------------:|:-------------------------------:
![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(512).png) | ![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Screenshot%20(514).png)




## RECOMMENDATION AND CONCLUSION
- From the report it's seen that Product Category 3 and 1 accounts for over 60% of revenue generated, so more effort should be put in to ensure it remains that way and cusotomers do not churn, thus quality and standard of product should be looking to imporve
- From forcast, sales for next year seems to be on the positive side, which is a good sig for the company ensuring all things stay equal.
- More research shouldbe carried out to uderstand why Product category 4 and 2 don't generte revenue as muxh as they were budgeted to, this insight would be incredibly helpful to know the next line of action to take to ensure revenue generation of the company increasees year by year. Possible solution could be improving marketing campaign. 


## Thank You
![](https://github.com/charlezvictor/Sales_Analysis_Viz/blob/main/Thank%20you.jpg)





I'm available to answer any questions and receive recommendation you have concerning this project.
Let's connect on [Linkedin](https://www.linkedin.com/in/victor-onyeaghala-08a909167/) and on [Twitter](https://www.twitter.com/_char_lez)
