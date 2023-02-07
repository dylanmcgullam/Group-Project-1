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
            2003-2011 - Invasion of Iraq
         

    

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
        
        1. Energy - Rebecca
        a/ Natural Gas: quoted in EUR/MMBtu.
        b/ Low Sulphur Gas Oil: quoted in EUR/MT.
        c/ WTI Crude: quoted in EUR/barrel.
        d/ Brent Crude: quoted in EUR/barrel.
        e/ ULS Diesel: quoted in EUR/gallon.
        f/ Gasoline: quoted in EUR/gallon.
        
        2. Industrial Metals - Chibuzor
        a/ Copper: quoted in EUR/lb.
        b/ Aluminum: quoted in EUR/MT.
        c/ Zinc: quoted in EUR/MT.
        d/ Nickel: quoted in EUR/MT.
       
        3. Precious Metals - Chibuzor
        a/ Gold: quoted in EUR/t oz.
        b/ Silver: quoted in EUR/t oz.
        
        4. Grains - Dylan
        a/ Corn: quoted in EUR/bushel.
        b/ Soybeans: quoted in EUR/bushel.
        c/ Wheat: quoted in EUR/bushel.
        d/ Soybean Oil: quoted in EUR/lb.
        e/ Soybean Meal: quoted in EUR/T.
        f/ HRW Wheat: quoted in EUR/bushel.
        
        5. Livestock - Dylan
        a/ Live cattle: quoted in EUR/lb.
        b/ Lean Hogs: quoted in EUR/lb.
        
        6. Softs - Rebecca
        a/ Sugar: quoted in EUR/lb. 
        b/ Coffee: quoted in EUR/lb. 
        c/ Cotton: quoted in EUR/lb. 
        
    Begin graphing prices over time for each sector.