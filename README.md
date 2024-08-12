# Business-360-Project

AtliQ Hardware has been on a rapid growth trajectory and is now taking a bold step by integrating data analytics through Power BI. This initiative is designed to not only outpace competitors but also to empower the company with data-driven insights across critical areas like finance, sales, marketing, and supply chain.
I played a key role in bringing this project to life, leveraging the expertise gained from the Codebasics Power BI Course. 

Live Report Link 

https://app.powerbi.com/view?r=eyJrIjoiMjI5YWE3MWUtM2Q4NS00ZWRiLWFjODItNTIyODAwMWU2OGNmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&embedImagePlaceholder=true/Readme.md

# Tech  stacks

* SQL
* PowerBi Desktop
* Excel
* DAX language
* DAX studio (for optimizing the report)
* Project charter file
* Data Modeling & Cleanning

# Technical Skills and Features to Implement:

* Creating Calculated Columns: Building custom columns to enhance data analysis.
* DAX Language for Measures: Crafting complex calculations and aggregations.
* Data Modeling: Structuring data relationships for optimal performance.
* Bookmarks for Visual Switching: Enabling seamless transitions between visuals.
* Page Navigation with Buttons: Enhancing user experience with intuitive navigation.
* Divide Function: Preventing division by zero errors for accurate calculations.
* Date Table Creation Using M Language: Generating a robust date table for time-based analysis.
* Dynamic Titles: Displaying titles that update based on applied filters.
* KPI Indicators: Using key performance indicators for quick insights.
* Conditional Formatting: Highlighting values in visuals with icons or background colors.
* Data Validation Techniques: Ensuring data accuracy and consistency.

# Power BI Services:
* Publishing Reports: Uploading reports to Power BI Services for sharing.
* Setting Up Personal Gateway: Automating data refresh for up-to-date reports.
* Power BI App Creation: Developing apps for streamlined access to reports.
* Collaboration, Workspace, and Access Permissions: Managing team collaboration and access controls in Power BI Services.

# Business Related Terms
* Gross price
* Pre-invoice deductions
* Post-Invoice deductions
* Net Invoice sale
* Gross Margin
* Net sales
* Net profit
* COGC - cost of goods sold
* YTD - Year to Date
* YTG - Year to Go
* Direct
* Retailer
* Distributors
* Consumer

# Company's Background
AtliQ Hardware has rapidly expanded its global footprint, opening new business ventures worldwide. Specializing in computers and accessories, the company operates through three key channels:
* retailers
* direct sales 
* distributors.
  
However, a recent misstep occurred when AtliQ opened a store in America based on intuition, surveys, and basic Excel analysis, resulting in unexpected losses. 
Meanwhile, competitors with robust analytics teams are making data-driven decisions, leaving AtliQ with no choice but to build its own analytics team to stay competitive and ensure future success.

In the project's kickoff session, it's crucial to clarify the purpose, goals, and any lingering questions to ensure a successful launch.

# Before Starting the Project: Key Questions to Ask:

* What are the primary objectives and goals of the project?
* Who are the key stakeholders, and what are their expectations?
* What data sources will be used, and how accessible are they?
* What are the timelines and deadlines for the project?
* What are the key performance indicators (KPIs) that need to be tracked?
* What resources and tools are available for the project?
* What are the potential risks or challenges, and how can they be mitigated?
* What level of data security and privacy is required?
* How will success be measured?
* What is the preferred format for the final deliverables?

# Understanding of Dataset
Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions

# gdb041:
   * dim_customer
	 * 27 distinct markets (ex India, USA, spain)
	 * 75 distinct customers thorough out the market
	 * 2 types of platforms
		* Brick & Motors - Physical/offline store
		* E-commerce - Online Store (Amazon, flipkart)
		* Three channels
			* Retailer
			* Direct
			* Distributors
   * dim_market
	* 27 distinct markets (ex India, USA, spain)
	* 7 sub-zones
	* 4 regions
	* APAC
        * EU
        * LATAM
  * dim_product
	* Divisions
	* P & A
	   * Peripherals
	   * Accessories
	* PC
	   * Notebook
	   * Desktop
	* N & S
	   * Networking
	   * Storage
	* There are 14 different categories, Like Internal HDD, keyboard
 	* There are different variants available for the same product
  * fact_forecast_monthly
	* This table is used to forecast the customer’s need in advance, which can help in
	     * Higher customer satisfaction
             * Reduced cost in warehouses for storage purpose
	* The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
	* All the date of the month will be replaced by the start date of the month
	* It will have all the column names and in the end it will have the forecast quantity need of the customer
  * fact_sales_monthly
	* This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.

# gdb056
  * freight_cost
	* This table has details of travel cost and other cost for each market with fiscal year
  * gross_price
	* Has the details of gross prices with product code
  * manufacturing_cost
	* Has the details of manufacturing cost with product code with year
  * Pre_invoice_dedutions
	* Has the details of pre invoice deductions percentage for each cutomer with year
  * Post_invoice_deductions
	* Post invoice deductions and other deductions details

# Importing data into Power BI
   * As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential.


# Data Model
* Data modeling is the foundation of any report, acting as the bedrock upon which all visuals are built.
* A well-structured data model is crucial because poor modeling can significantly impact the overall performance of the report.
* Adhering to best practices in data modeling is essential to ensure efficiency and accuracy. 
* In this project, we adopted the Snowflake data modeling approach to ensure optimal performance and scalability.
  
![image](https://github.com/user-attachments/assets/16c37914-4d39-454c-8589-f6dbdedd388f)

# Dashboard Designing 
Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required.

# Dashboard HOME View
In Home view, all the views button will be available. User will land on specific view page by clicking the button

* Info
* Finance View
* Sales View
* Marketing View
* Supply chain View
* Executive View
* Support

# Home View
![image](https://github.com/user-attachments/assets/15131b78-02b7-4b51-a5fb-5f6bf3d3077d) 

# Info View
![image](https://github.com/user-attachments/assets/c9b0597a-5281-4ee6-9fd8-20d2f3b6af18)

# Finance View
![image](https://github.com/user-attachments/assets/bf4abe3b-af23-44a5-ae23-10c39f55d0e5)

# Sales View
![image](https://github.com/user-attachments/assets/2ee28507-19e5-4b96-aa73-2233f8e5934c)

# Marketing View 
![image](https://github.com/user-attachments/assets/524b10dc-2c32-4d0b-b464-f771a736e1b9)

# Supply Chain View
![image](https://github.com/user-attachments/assets/10d555e8-0947-4ed3-80d0-c1f70fef3276)

# Executive View
![image](https://github.com/user-attachments/assets/42ea7f13-da46-47d0-8be1-40fa83516231)

# Support
![image](https://github.com/user-attachments/assets/2d28da4c-806b-4ea9-acc3-e363eb741bda)


# Project Outcome
This report enables data-driven decision-making, allowing for in-depth analysis and providing answers to various 'why' questions based on specific situations.


















