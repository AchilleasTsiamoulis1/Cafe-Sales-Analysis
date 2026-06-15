# Cafe-Sales-Analysis
* In this Data Analysis session I chose a dirty dataset from Kaggle that was based on Cafe Sales, I cleaned the data inside the Excel file and then used Tableau to visualize the results. 
* The original dataset was downloaded from https://www.kaggle.com/datasets/ahmedmohamed2003/cafe-sales-dirty-data-for-cleaning-training 
# Data Preparation & Data Cleaning 
To start with, as soon as I downloaded the dataset, it needed some processing before the columns and their data became visible.

* I selected the first column -> Data -> Text to Columns -> Delimited by comma
* CTRL A -> ALT -> Type HOI
* Bold the column headers.

Then it was time for the **Data Cleaning**. This dataset was not something really hard to deal with. It includes 8 columns. **Transaction ID, Item, Quantity, Price Per Unit, Total Spent, Payment Method, Location and Transaction Date**. Personally, I do not like having IDs like this TXN_1961373. I prefer only numbers so I created a new column with the name **New_ID** and with the function **RIGHT** I chose to keep only the last 7 digits. 

Next, I noticed that every other column contains **blanks** and data called **UNKNOWN** and **ERROR**. In order to delete them I chose **Filter** from the **Data tab**, unselect the correct data and select only the one I want to delete. Then, I chose every row and delete it. This is it, the dataset is ready to be used for analysis. There were no duplicates, no issues with the dates, no columns that needed to be deleted, no questions with words that contained both uppercase and lowercase letters so you had to normalize them.
