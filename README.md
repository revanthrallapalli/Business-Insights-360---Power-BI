# Business-Insights-360-Power-BI
Created Dashboard by using tools such as Power BI, Excel and SQL. 

# Project Overview

🔸AtliQ Hardware is a hardware manufacturing company that offers a variety of hardware products to customers across different countries. As a rapidly growing company, AtliQ Hardware faced the challenge of efficiently collecting and analyzing data from various sources such as SQL databases, Excel spreadsheets, and CSV files. Their ability to make informed business decisions for sustainable expansion may be hindered by these obstacles and take appropriate corrective measures.\
🔸Task - Develop an interactive report that provides valuable insights to finance, sales, marketing, supply chain, executive and product teams, using the provided mock-up dashboard as a reference.

Please visit the live interactive dashboard in below link\
[Live Report Link](https://www.novypro.com/profile_about/revanth-rallapalli?Popup=memberProject&Data=1727214193102x603097518925027200)

# Tools Used
* SQL
* PowerBi Desktop
* Excel
* DAX language
* DAX studio (for optimizing the report)
* Project charter file

# Power BI techniques learnt such as:
✅Data modelling\
✅Creation calculated tables and columns\
✅Creation measures using DAX language\
✅Creation data tables using M-language\
✅Use Bookmarks to toggle between two visuals\
✅Use tooltips to display data\
✅Use Page navigations with buttons\
✅Creation of KPI indicators\
✅Use Dynamic titles based on applied filters\
✅Use conditional formatting of values in visuals\
✅Data validation techniques\
✅Publish report to Power BI Services\
✅Setting up the personal gateway to set up the auto-refresh of data\

# Business Related Terms:
✅ Gross price\
✅ Pre-invoice deductions\
✅ Post-Invoice deductions\
✅ Net Invoice sale\
✅ Gross Margin\
✅ Net sales\
✅ Net profit\
✅ COGC - the cost of goods sold\
✅ YTD - Year to Date\
✅ YTG - Year to Go\
✅ Ads and Promotions\

# AtliQ Company’s background
AtliQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel
* Retailers
* Direct
* Distributors

Recently the company has faced a unforeseen loss by opening store in Latin America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AtliQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry.\
The report's objectives were discussed by AtliQ professionals during the project kick-off meeting. Based on requirement, the data engineering team has given the data as per the request of data analytics team, let’s explore them.\

# Dataset Understanding
Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.\

Dimension table : It will have the static data like details of customer and products\

Fact table : It will have the data about the transactions

* gdb041:
  * dim_customer
      + 27 distinct markets (ex India, USA, Spain etc.)
      + 75 distinct customers thorough out the market
      + 2 types of platforms
          + Brick & Motors – Physical/offline store
          + E-commerce – Online Store (Amazon, flipkart)
      + Three channels
          + Retailer
          + Direct
          + Distributors
  * dim_market
      + 27 distinct markets (ex India, USA, spain)
      + 7 sub-zones
      + 4 regions
          + APAC
          + EU
          + nan
          + LATAM
  * dim_product
      + Divisions
          + P & A
              + Peripherals
              + Accessories
          + PC
              + Notebook
              + Desktop
          + N & S
              + Networking
              + Storage
    + There are 14 different categories, Like Internal HDD, keyboard
    + There are different variants available for the same product
  * fact_forecast_monthly
    + This table is used to forecast the customer’s need in advance, which can help in
        + Higher customer satisfaction
        + Reduced cost in warehouses for storage purpose
    + The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
    + All the date of the month will be replaced by the start date of the month
    + It will have all the column names and in the end it will have the forecast quantity need of the customer
  * fact_sales_monthly
    + This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
  * gdb056
    * freight_cost
      + This table has details of travel cost and other cost for each market with fiscal year
    * gross_price
      + Has the details of gross prices with product code.

    * manufacturing_cost
      + Has the details of manufacturing cost with product code with year
    * Pre_invoice_dedutions
      + Has the details of pre invoice deductions percentage for each cutomer with year
    * Post_invoice_deductions
      + Post invoice deductions and other deductions details

# Importing data into PowerBi
* As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential

# Data Modelling
* Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
* Poor data modeling affects the over all performance of the report.
* In this project, we have followed Snowfall data modeling method.

![Data Model](https://github.com/user-attachments/assets/12338734-3538-4f41-a2ee-675e0cf9b11b)


# Dashboard designing
Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

# Home view
In Home view, all the views button will be available. User will land on specific view page by clicking the button.
* Info
* Finance View
* Sales View
* Marketing View
* Supply chain View
* Executive View
* Products
* Support

# Info
![Info_slide](https://github.com/user-attachments/assets/926c5090-edc6-48d5-b467-74a681b12dd4)

# Finance View
![finance_slide](https://github.com/user-attachments/assets/23b4aa23-6525-4801-b0be-26deb7bf21bf)

# Sales View
![sales_slide](https://github.com/user-attachments/assets/6fb889f2-558c-4df2-90e1-c0a08e9053ea)

# Marketing View
![marketing_slide](https://github.com/user-attachments/assets/2c57b3ff-6e65-4ab0-b4d5-f4601815faa7)

# Supply Chain View
![Supply Chain_slide](https://github.com/user-attachments/assets/fc407d96-7f0d-4b38-adf6-79d8eab29cb5)

# Executive View
![executive_slide](https://github.com/user-attachments/assets/575feeaf-705b-4664-8653-1bb09b062c23)

# Products View
![product_slide](https://github.com/user-attachments/assets/2428a247-cb4e-483f-a0e5-a692d5dba838)

# Overall Report
you can find the full report file here : [Report](https://www.novypro.com/profile_about/revanth-rallapalli?Popup=memberProject&Data=1727214193102x603097518925027200)

# Project Outcome
By using this report, decisions can be taken based on the data. Further it will help in answering and number of why questions based on the situations.









