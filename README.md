# Final-project-Wasp

# Essential Files 
    1. Fortune.csv : This file contains our primary dataset
    2. CleanedFortune.csv: This file is the same file as Fortune.csv after performing data cleaning
    3. S&P500.csv: This file is our secondary dataset, obtained by scraping.
    4. Cleaned_S&P500: This is the same file as S&P500.csv after performing data cleaning
    5. Data Cleaning.ipynb: This file contains the data cleaning code for both the datasets
    6. EDA.ipynb: This file contains the EDA for both Datasets
    7. FinalWebScraping.ipynb: Contains the scraping code for S&P500 dataset. This file might not open on github. However,
        it can be viewed on the below link:
        https://raw.githubusercontent.com/CS-UCR/final-project-wasp/master/WebScraping.ipynb?token=ANLGLKHKUQGY323TMYAYRNC7DZPHA
    8. Regression.ipynb: Contains the visuals related to Linear Regression and AshenFelter's Model (Phase3) 
    
# Datasets

In our project, we have obtained two Datasets. The primary Dataset is Fortune500 which containes the information of the top 500 companies in the years 2017, 2018, and 2019. This dataset provides all the essential financials of a company, such as the value of its revenues, value of its assets, their profits/losses, number of employees at each company, and various other information. Our primary analysis is done on this dataset. Our analysis includes the comparison of the several different attributes of each company. For instance, one of our analysis included on how how the companies profits are correlated to their Revenues. We obtained this dataset online which was readily available to download.

# Scraper

Our second Dataset was obtained by web scraping. This scraper obtained the information about the S&P 500 companies and how their stock prices have fluctuated from each day's trading session. The data scraped included the name of the company, its stock symbol, the weight, the price, the change in the price from the previous trading day, as well as the percentage change in price. The entire dataset was on one page, hence, there was no need to iterate through different pages while scraping the data.

This dataset includes 505 symbols, however it is suppose to contain 500. This is due to the fact that several companies have two share classes. For example, Google's parent company Alphabet has Class A (GOOGL) and Class C (GOOG) shares in the index. The primary purpose of this Dataset was to fulfill the Data collection component of the project. 

# Team Contributions

Shawn worked primarily on the Web Scraper while I (Saad Umar) worked mostly on the EDA and data cleaning, however, we both helped each other out during the process. As we proceeded to phase 3 of the project, both of us worked towards Linear Regression and the Ashenfelter's Model. Shawn mostly worked on the S&P500 dataset, while I mosly worked on the Fortune500 dataset.

# Running the Code/ dependencies

* Open any environment that allows Jupyter Notebooks

* Download the relevant CSV files. They can be either downloaded/ or cloned from our githib repo.

* Open the Data Cleaning.ipynb file and run it. Its important to run this file before others in order to perform EDA on the cleaned data.

* Open the EDA.ipynb file or the Regression.ipynb file and run them.

* Click on the 'Kernel' option which opens another list of options.

* Click "Restart Kernel and run all cells" in order to run the notebook.

# Analysis Summary for Phase 3

As we moved to Phase3, we used Linear Regression and the Ashenfelter model on the fortune500 dataset. Our primary goal was to see what features affects a company's rank. Thus, "Rank" was our target variable. Some of the questions we wanted to answer using this analysis are as follows:

    1. How do the Number of Employees in a Company affects its ranking on the Fortune500?
    2. How do the Revenues of a Comapny affects its ranking on the Fortune500?
    3. How do the Assets of a Comapny affects its ranking on the Fortune500?
    4. How do the Profits of a Comapny affects its ranking on the Fortune500?
    
The in-depth answers to the above questions can be found in the Regression.ipynb notebook with relevant visuals. However, we can summarize some of our analysis below.

When comparing the affect of Number of Employees on the ranking (target), we did not see any meaningful information. The company rankings were widely spread throughout the scatter plot, even though most of the companies almost had the number of employees. We then compared how the revenues of a company affected its ranking. We noticed that as the revenue increases the rank (value) decreases (negatively correlated). The rank value decreases means that the company is ranked higher. Additionally, the profits and assets did not show any meaningful visuals on how they affected a company's ranking. So from this information we were able to conclude that the "Revenue"(feature) had the most weight on how it affects a company's ranking (target). Furthermore, when we applied the Ashenfelter model with the Revenue, Assets, Profits, and Number of employees as features and the Ranking as target, we noticed that all the revenue, profits, and assets were negatively correlated to a company's ranking. This means that the predicted target(rank value in our case) decreases as the features value increases. This means that comapanies that were highly ranked had a higher revenue. However, the "Number of Employees" was positvely correlated to the rank.

# Problems we encountered during the project

The biggest problem we encountered was related to web-scraping on which we invested alot of time. However, we realized that the Fortune500 website had javascript enabled content (dynamic), hence, it was not scrapable with the current resources/libraries we had. Thus, we went ahead and scraped the S&P500 dataset from the following url: https://www.slickcharts.com/sp500

