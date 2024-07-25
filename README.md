# Snapshot of top 25 active Canadian stocks on Yahoo stocks

## Project Overview
This data analysis project aims to provide a snapshot of top 25 active Canadian stocks on July 20th, 2024. By using various aspects of Python and web scrapping, I am showcasing my skillset of Python, web scrapping, Jupyter and Pandas. 

### Data Source
This data is directly sourced from [https://finance.yahoo.com/most-active/]. It contains detail information regarding active stocks recommended by Yahoo Finance.

### Tools
- Python
- Web Scrapping
- Jupyter library
- Pandas Library

### steps taken 

#### BeautifulSoup and Requests

- Imported BeautifulSoup and requests in Jupyter library
- Copied and renamed the URL from where I was sourcing my data
- Used requests command to check if I can go ahead and get this data
- Used BeautifulSoup to import all data from the webpage
- Used inspect element to find the exact table that I want to import from the HTML code of the webpage and renamed it as table
- Used inspect element once again to find the titles of the table from HTML code of the webpage
- Deleted some titles which are not useful for this project or are not supported by Jupyter

#### Pandas 

- Imported pandas as pd and renamed the titles I got earlier as df
- Checked if all column titles are imported correctly
- Now went back to inspect element to check the code and find body of the table (rows data)
- Found the body of the table and imported it
- Manually manupilated the row data into 25 smaller list for each stock
- After that I assigned the rows to its appropriate columns and called out df to get an exact snapshot of the webpage data table.


### Limitation

- Yahoo uses 1 big list for all of its data in the table instead of smaller individual list per stock, I had to manually adjust each list to fall into its column.
- Also, as I had to delete some title columns, each stock had to be adjusted individually to its column which took some time. 
