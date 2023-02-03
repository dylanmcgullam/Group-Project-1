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
        Data trends during/after COVID-19
        Effects of war(s)
        Effects of Hurricane Harvey on global market
    

Datasets to Be Used
    https://www.kaggle.com/datasets/debashish311601/commodity-prices

Rough Breakdown of Tasks







#Steps Taken
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