# Cafe-Sales-Analysis
* In this **Data Analysis** session I chose a dirty dataset from **Kaggle** that was based on **Cafe Sales**, I cleaned the data inside the **Excel** file and then used **Tableau** to visualize the results. 
* The original dataset was downloaded from https://www.kaggle.com/datasets/ahmedmohamed2003/cafe-sales-dirty-data-for-cleaning-training
* I have also provided both the original dateset and the one I have modified.
* If there is an issue on the Tableau file after downloading it, here is the link for the Tableau Public to check it out https://public.tableau.com/views/CafeSales_17815405813140/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link 
# Data Preparation & Data Cleaning 
To start with, as soon as I downloaded the dataset, it needed some processing before the columns and their data became visible.

* I selected the **first column** -> **Data** -> **Text to Columns** -> **Delimited by comma**
* **CTRL A** -> **ALT** -> Type **HOI**
* **Bold the column headers.**

Then it was time for the **Data Cleaning**. This dataset was not something really hard to deal with. It includes 8 columns. **Transaction ID, Item, Quantity, Price Per Unit, Total Spent, Payment Method, Location and Transaction Date**. Personally, I do not like having IDs like this TXN_1961373. I prefer only numbers so I created a new column with the name **New_ID** and with the function **RIGHT** I chose to keep only the last 7 digits. 

Next, I noticed that every other column contains **blanks** and data called **UNKNOWN** and **ERROR**. In order to delete them I chose **Filter** from the **Data tab**, unselect the correct data and select only the one I want to delete. Then, I chose every row and delete it. This is it, the dataset is ready to be used for analysis. There were no duplicates, no issues with the dates, no columns that needed to be deleted, no questions with words that contained both uppercase and lowercase letters so you had to normalize them.

# Tableau Analysis
In Tableau, I created 4 different sheets, which I then consolidated into a single dashboard, exactly as shown.

The first sheet (top left) shows the products customers purchase at coffee shops, broken down by quantity. Salad and juice are the top-selling products.

The second sheet (bottom left) presents the two different options available to customers—takeout or dine-in—in combination with the quantity of the product. 
Essentially, this is an extension of the previous sheet. In-store, the salad and juice remain the top sellers, while for takeout, cookies and coffee lead the way—which makes sense objectively.

The third sheet (top right) is a chart divided into three sections based on customers’ payment methods (cash, credit card, digital wallet), showing in ascending order the products they buy most frequently. Salad remains at the top for cash and credit card payments, but juice takes first place for digital wallet payments.

The fourth and final sheet (bottom right) shows the price of the product people buy most often—that is, the product costing 3 units has been purchased most frequently.
Finally, all of the above sheets have been arranged uniformly in an interactive dashboard where the other charts change depending on what the user clicks.

The first sheet is a stacked bar chart.

The second sheet is a side-by-side bar chart.

The third sheet is a line chart.

The fourth sheet is a pie chart.
