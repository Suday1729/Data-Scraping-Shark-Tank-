# Data-Scraping-Shark-Tank-
Scraping of offers table from (Shark Tank) website (Contains jupyter file, dataset)

Procedure
•	Changed working directory to the folder containing selenium script
•	Imported the necessary libraries
•	Inspected the webpage to locate the “offers table” in the webpage
•	Once the table was located, the column header names was passed to ‘thead’ variable
•	All the row elements were extracted using loop function and find_all('tr'), find_all('td')
•	Reusable function was defined (shark_table(table_no)) which takes input argument as the required table in the webpage
•	Checked whether the shark_table(table_no)) function was able to scrap all tables in the webpage
•	Using the shark_table(table_no)) function, dataframe (tab3) was defined which contained the details of “offers table”
•	tab3 dataframe was converted to .csv file as “Shark Tank Offers Table.csv” 

Challenges
•	While defining the reusable function, there was an issue caused by the “thead” variable which contained the column header names of tables
•	Out of the 3 tables in the webpage the first table did not have column header names, which created an empty list for “thead”
•	Resolved the issue using “if condition” statement in the function

