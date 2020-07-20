# Final-project-Wasp

# Essential Files 
    1. Fortune.csv : This file contains our primary dataset
    2. CleanedFortune.csv: This file is the same file as Fortune.csv after performing data cleaning
    3. S&P500.csv: This file is our secondary dataset, obtained by scraping.
    4. Cleaned_S&P500: This is the same file as S&P500.csv after performing data cleaning
    5. Data Cleaning.ipynb: This file contains the data cleaning code for both the datasets
    6. EDA.ipynb: This file contains the EDA for both Datasets
    7. WebScraping.ipynb: Contains the scraping code for S&P500 dataset. This file might not open on github. However,
    
        it can be viewed in the "Raw" mode on github. or on this link:
        
        https://raw.githubusercontent.com/CS-UCR/final-project-wasp/master/WebScraping.ipynb?token=ANLGLKHKUQGY323TMYAYRNC7DZPHA
    
# Datasets

In our project, we have obtained two Datasets. The primary Dataset is Fortune500 which containes the information of the top 500 companies in the years 2017, 2018, and 2019. This dataset provides all the essential financials of a company, such as the value of its revenues, value of its assets, their profits/losses, number of employees at each company, and various other information. Our primary analysis is done on this dataset. Our analysis includes the comparison of the several different attributes of each company. For instance, one of our analysis included on how how the companies profits are correlated to their Revenues. We obtained this dataset online which was readily available to download.

# Scraper

Our second Dataset was obtained by web scraping. This scraper obtained the information about the S&P 500 companies and how their stock prices have fluctuated from each day's trading session. The data scraped included the name of the company, its stock symbol, the weight, the price, the change in the price from the previous trading day, as well as the percentage change in price. The entire dataset was on one page, hence, there was no need to iterate through different pages while scraping the data.

This dataset includes 505 symbols, however it is suppose to contain 500. This is due to the fact that several companies have two share classes. For example, Google's parent company Alphabet has Class A (GOOGL) and Class C (GOOG) shares in the index.

The primary purpose of this Dataset was to fulfill the Data collection component of the project. Shawn worked primarily on the Web Scraper while I (Saad Umar) worked mostly on the EDA and data cleaning, however, we both helped each other out during the process.

# Running the Code

* Open any environment that allows Jupyter Notebooks

* Download the relevant CSV files. They can be either downloaded/ or cloned from our githib repo.

* Open the EDA.ipynb file, which reads the csv files 

* Run "Restart Kernel and run all cells" from the 'Kernel' option to run the file



