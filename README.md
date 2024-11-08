# Brand Analysis 

### Project Overview

This project focuses on analyzing Hyundai's position in the car sales market, using data from Turbo.az to evaluate its performance relative to competitors. 
The goal is to identify market trends, assess Hyundai's sales strategies, and leverage insights from social media for targeted growth initiatives.


### Data Sources

Data used in task was obtained from kaggle:

[download here](https://www.kaggle.com/code/isazeynalov/turbo-az-web-scraping-and-cleaning/input)



### Tools

- MS SQL - Data manipulation
- Power Query - Data Processing
- Power BI - Creating Reports



### Data Collecting and Manipulating


- MS SQL

  
 **1. Creating [Car_sales_db] database using SSMS.**

 **2. Importing [dbo].[Turbo.az_car_data] file from excel through wizard using SSMS.** 
   
   -- select * from [dbo].[Turbo.az_car_data] 


 **3. Separating name into brandname and modelname in order to get deep information about brand.**
 PS. There could be some mistakes due to existence of two spaces in brand name,
 but for our target brands(hyundai, mercedes, toyota etc) everything is okay.      


   /*   alter table [dbo].[Turbo.az_car_data]
    add brandname nvarchar(30), modelname nvarchar(30) */

   /*   update [Turbo.az_car_data] 
   set --brandname = left(name, charindex(' ', name) - 1)
   modelname = substring(Name, charindex(' ', name) + 1, len(Name))   */




### Creating Reports

After this step, all processes will be done through power query and power bi.


**4.Importing that data via “Get data” from SQL Server.**

**5. Market Analysis - Focused on overall market conditions and competitors.**

- Top brands by count of sales and sales amount.
- Market share by Engine type
- Cards for statistic measures and sales details.


  **Brand Analysis - Analysis of our brand to improve growth strategy.**

- Count of sales by model and release year
- Sales amount by model
- Statistic measures and sales details.
  Social Media Review - Insights and metrics from Social Media Analytics tools and sites such as Instrack, BrandMentions, Brand24 etc. 

 **Social Media Analytics and Monitoring Metrics for Instagram and Web**
- Most used hashtags
- Some mentions from web about brand



**Note: Prices are expressed as dollars.**



