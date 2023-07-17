# Maven Market Data Visualization Using Power BI Desktop


## Objective:
- Maven Market, a multi-national grocery chain with locations in Canada, Mexico and United States have provided us their 1997-1998 Sales and Returns data.
- As a Data Analyst, we need to create Key Performance indicators to check if company is growing or declining. And also see the trends of their Sales data annually or monthly or weekly.

## Tool:
Power BI Desktop

## BI Workflow followed:
1. connecting and shaping the data --> 2. building a relational model --> 3. adding calculated fields using DAX --> 4. designing an interactive report.

### Step 1: Connecting and shaping data
- Here we load the csv files that was provided and transform the data to remove duplicates/ blanks/ or any error row columns using Power Query.
- Using View --> Column Quality we can check if there's any duplicates or blanks left.
- Then we check all columns data types manually and change it using auto detect or manually if needed.
- Add new columns which are required to obtain our goal objective like for 'Calendar' file we only have date , we added columns like start of month, start of week, month name and also using IF condition to create a weekday/weekend based on day.
- We can remove unwanted columns from tables and also if any file doesn't change much we can stop it from refreshing which increases BI tools performance.
- Once all the data cleaning and transformation is done we can use "Close and Apply" to load the data into "Power BI front end".

### Step 2: Building a relational model.
- Here we connect all the fact and dimension tables into either "Star Schema" or "Snowflake Schema" using tables primary and foreign keys.
- Always make sure that dimension table to fact table relations should be (1 to many) and try to avoid bi-directioal filters if not necessary as they create ambiguity.

![image](https://github.com/shubham-shetty12/Maven_Market_Data_Visualization/assets/137090796/a65b7513-02db-4170-b500-d813d122c1d6)


### Step 3: Adding Calculated fields using DAX:
- We will create a new table 'Measures' to store all our key metrics and calculated fields using DAX inside this table to avoid mess and its easy to select all needed fields from single table than finding it in individual tables.
- Below are some of the useful measures created using DAX.

![image](https://github.com/shubham-shetty12/Maven_Market_Data_Visualization/assets/137090796/970799d7-df0e-494e-97df-edf8f55eef46)

### Step 4: Creating interactive visualization report:
- We have lot of visual tools available and can use any of them as per interest.
- I have used some basic visuals like Cards, line chart,stacked bar chart, Donut chart, Matrix, Slicer, Map and Guage.
-  Below is the final view of Dashboard.

![image](https://github.com/shubham-shetty12/Maven_Market_Data_Visualization/assets/137090796/929dc2c5-870a-4d21-b4a3-6c80614ec8f9)

 


 
