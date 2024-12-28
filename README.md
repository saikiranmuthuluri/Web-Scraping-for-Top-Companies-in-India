# Web-Scraping-for-Top-Companies-in-India

**Project Overview**

This project demonstrates how to scrape data from the Wikipedia page listing the largest companies in India. The script fetches the webpage content, parses the HTML using BeautifulSoup, extracts the relevant information from a table, and stores it in a CSV file for further analysis.

**Features**

**Data Extraction:** Extracts details such as the company name, industry, and revenue from the table on the Wikipedia page.
**Data Storage:** Saves the extracted data in a structured CSV format using the Pandas library.
**Web Scraping:** Uses the requests library to fetch HTML content and BeautifulSoup for parsing and data extraction.


**Requirements**

**requests library:** Used for making HTTP requests to fetch webpage content.
**BeautifulSoup library:** Used for parsing and extracting data from HTML content.
**pandas library:** Used to store and manipulate the extracted data in a tabular format.


**Code Walkthrough**

    **Importing Required Libraries:** The script begins by importing the necessary libraries: requests, BeautifulSoup from bs4, and pandas.
    
    **Defining the URL:** The URL of the target webpage is specified: "https://en.wikipedia.org/wiki/List_of_largest_companies_in_India". This page contains a table with a list of the top companies in India.
    
    **Sending a Request to the Webpage:** The script sends an HTTP GET request to the specified URL and checks if the response status is 200 (OK). If the status code is different, it exits the program.
    
    **Parsing the Webpage Content:** The content of the webpage is parsed using BeautifulSoup, which allows for easy navigation and extraction of data from the HTML structure.
    
    **Extracting the Table Data:** The script searches for the second table in the webpage and extracts the column headers (titles). It then parses each row of the table, extracting the data and storing it in 
      a DataFrame.
    
    **Saving the Data:** After extracting the required data, it is stored in a CSV file (Companies.csv) using the pandas DataFrame.


**Output**:

The script will generate table format and csv file containing information about the top companies in India, including details such as company name, industry, and revenue.

**Example Output:**

   Company Name: Reliance Industries
  
   Industry: Conglomerates
  
   Revenue: ₹6.57 trillion

**Conclusion**

This project showcases a simple and effective way to extract structured data from a website using Python, requests, BeautifulSoup, and pandas. The scraped data can be used for further analysis, reporting, or visualization.
