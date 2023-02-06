# Group-Project-1

Project Title
    Commodity in Action

Team Members - Group 5
    Rebecca Davidson
    Chibuzor Ejiaga
    Dylan McGullan

Project Description/Outline


Research Questions to Answer
    Volatility of prices
        Data trends during 2008 Recession
            December 2007 to June 2009
        Data trends during/after COVID-19
            January 2020 to August 2021
        Effects of war(s)
            9/11/2001 - Invasion of Afghanistan
            2003-2011 - Invasion of Iraq
            2014 - U.S.-led intervention in Syria
            February 24, 2022 - Russian invasion of Ukraine
        Effects of weather on global market
            August 25-29, 2017 - Hurricane Harvey
            August 23, 2005 - Hurricane Katrina
    

Datasets to Be Used
    https://www.kaggle.com/datasets/debashish311601/commodity-prices

Rough Breakdown of Tasks







Steps Taken:
Imported CSV file.
Set DATE columns as the index.
Replaced Nan with 0.
Converted prices from EUR to USD.
Renamed columns.
Ran aggregate function to get "mean", "median", "var", "std", "sem".
Started exploring boxplots to look at outliers.
Next steps:  
    Create separate dataframes for each of the following sectors:  Energy, Industrial Metals, Precious Metals, Grains, Livestock, and Softs.
    Begin graphing prices over time for each sector.