# Final-project-Wasp

* Team Members:
    1. Saad Umar
    2. Shawn Rahlwes
    
# Datasets

In our project, we have obtained two Datasets. The primary Dataset is Fortune500 which containes the information of the top 500 companies in the years 2017, 2018, and 2019. This dataset provides all the essential financials of a company, such as the value of its revenues, value of its assets, their profits/losses, number of employees at each company, and various other information. Our primary analysis is done on this dataset. Our analysis includes the comparison of the several different attributes of each company. For instance, one of our analysis included on how how the companies profits are correlated to their Revenues. We obtained this dataset online which was readily available to download.

# Scraper

Our second Dataset was obtained by web scraping. This scraper obtained the information about the S&P 500 companies and how their stock prices have fluctuated from each day's trading session. The data scraped included the name of the company, its stock symbol, the weight, the price, the change in the price from the previous trading day, as well as the percentage change in price. The entire dataset was on one page, hence, there was no need to iterate through different pages while scraping the data.

This dataset includes 505 symbols, however it is suppose to contain 500. This is due to the fact that several companies have two share classes. For example, Google's parent company Alphabet has Class A (GOOGL) and Class C (GOOG) shares in the index.

The primary purpose of this Dataset was to fulfill the Data collection component of the project.

# Running the Code

* Open any environment that allows Jupyter Notebooks

* Download the relevant CSV files (Fortune.csv) which is the uncleaned version or the (CleanedFortune.csv), the cleaned  version. Can be downloaded/ or cloned from our githib repo.

* Open the EDA.ipynb file, which reads the CleanedFortune.csv

* Run "Restart Kernel and run all cells" from the 'Kernel' option to run the file



