# Project_2
Crowdfunding_ETL-challenge
Project Partners: Lwam Mehare, Rebecca Solomon, Rosanna Chiu, Yi Pan, Telmen Erdenebat and Harsh Chapadia.

Note: For the partners project my group and I discussed the deliverables and each completed the code independently. There are separate repos and separate notebooks, scripts with the work.

# Project Overview:
Building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions after transforming the data, create 4 CSV files and use the CSV file data to create an ERD and a table schema load CSV files to resources db the overall project is broken into 4 subsections.

Subsection 1: Create Category, Subcategory Dataframes
Subsection 2: Create a Campaign DataFrame:
Subsection 3: Create a Contacts DataFrame:
Subsection 4: Create the Crowdfunding database:

# Subsection 1: Create Category, Subcategory Dataframes
Extract and transform the crowdfunding.xlsx data to create a dataframe for category the category dataframe should contain only 2 columns -- category and a new category_id ** the category_id column should contain entries going sequentially from "cat1 to catn" and relates to the number of unique categories export the category dataframe to a CSV file extract and transform the crowdfunding.xlsx data to create a dataframe for subcategory the subcategory dataframe should contain the distinct list of subcategories from the crowdfunding excel file and a list of subcategory_ids, created within the dataframe export the subcategory dataframe to a csv file.

# Subsection 2: Create a Campaign DataFrame:
Extract and transform the crowdfunding.xlsx to create a campaign DataFrame: "cf_id" column "contact_id" column "company_name" column "blurb" column, renamed to "description" "goal" column, converted to the float data type "pledged" column, converted to the float data type "outcome" column "backers_count" column "country" column "currency" column "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format "category_id" column "subcategory_id" column export campaign dataframe to csv

# Subsection 3: Create a Contacts DataFrame:
Extract and transform data from the contacts sheet. Data was extracted using both the python dictionary method and the regular expression Python Method: load excel file to data frame iterate through data frame using either nested for loop or list comprehension extract the dictionary values from the keys by using a Python list comprehension. Add the values for each row to a new list Create a new DataFrame that contains the extracted data Split each "name" column value into a first and last name, and place each in a new column. export data frame to csv file

# Subsection 4: Create the Crowdfunding database:
Inspect the 4 csv files and create an ERD of the tables export the ERD diagram and table schema and load to repository create a new postgres database - crowdfunding_db create a table schema for each of the CSV files Save the database schema as a Postgres file named crowdfunding_db_schema.sql, Using the database schema, create the tables in the correct order to handle the foreign keys. load csv files to respective tables within the database and confirm tables return records
