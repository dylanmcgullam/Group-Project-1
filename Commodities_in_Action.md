Commodities in Action
    by:  Rebecca Davidson, Chibuzor Ejiaga, & Dylan McGullan


For this project, we chose to focus on commodities and how different historical events have impacted those commodity prices.  Our questions to answer are the following:
    What effect does war have on commodity prices?
    What effect does an economic crisis have on commodity prices?
    What effect does a health crisis have on commodity prices?
We pulled a dataset from kaggle.com that contained commodity prices from early 2000 to late 2022.  We looked at the data as a whole, then divied up the workload by sector and by historical event.  The breakdown is the following
    
    Rebecca:    Energy Commodities during the Invasion of Iraq in (03/2003 to 12/2011)
                    Natural Gas
                    Low Sulphur Gas Oil
                    WTI Crude
                    Brent Crude
                    ULS Diesel
                    Gasoline
                Soft Commodities during the Invasion of Iraq (03/2003 to 12/2011)
                    Sugar
                    Coffee
                    Cotton

    Chibuzor:   Metal Commodities during the 2008 Recession (12/2007 to 06/2009)
                    Copper
                    Aluminium
                    Zinc
                    Nickel
                    Gold
                    Silver

    Dylan:      Agricultural Commodities during COVID-19 (01/2020 to 08/2021)
                    Corn
                    Soybeans
                    Wheat
                    Soybean Oil
                    Soybean Meal
                    HRW Wheat
                    Live Cattle
                    Lean Hogs

We cleaned up the original dataset, replacing empty cells with 0, and formatting the date column as the index.  We also converted the prices from EUR to USD by using a 1.09 conversion rate.  During the data cleaning process, we discovered the gasoline prices between the years 2000 to 2005 were missing and we replaced them with 0.  We are aware that would skew the data.  We also discovered that several of these commodity price values were amplified by a factor of 100. Soybeans, corn, ULS diesel, wheat, gasoline, and coffee were all off by roughly a factor of 100.  Instead of changing the dataset by dividing those values by 100 or dropping those commodities altogether, we decided to still use the raw data because while the values are off, the data would still represent the general trend of that commodity price. 

Our first visual is a graph showing all prices for all commodities for the years 2000-2022.  The three historical events we are focusing on are annotated on the plot.  The first takeaway from the plot is that nickel sits way higher than all the other commodities, making it difficult to see the rest of the data.

After this, we ran the .agg function on the dataset to get the mean, median, variance, standard deviation, and standard error of the mean over the entire 22-year period.  We plotted boxplots on the whole dataset, but it was difficult to analyze the plot because all the commodities are on such a wide range of prices.  From this point, we each focused on our sectors and historical event.

Energy Sector
I pulled all 6 energy commodities from the main dataframe and created a separate dataframe.  I ran the .agg function on it.  Then I used the .loc function to pull data within a date range to focus on the Invasion of Iraq that occurred between 2003-2011.  I plotted this daily data, along with the mean of each over the 22-year period.  This would show how the daily data over this specific time period compared to the 22-year mean.  During the Invasion of Iraq, energy commodities generally had an upward trend.  The 2008 Recession did occur during this time period also, but on average, the trend was in the positive direction and much of it sat above the 22-year mean.  While the immediate response to the invasion dropped prices, they eventually increased and peaked right before the 2008 Recession, only to drop again.  Energy prices slowly increased and when the war was over in 2011, prices seemed to stabilize.

Metal Sector 
I pulled the 6 commodities from the main dataset and created another one specifically for metals. After I determined this, I used an .agg and a .loc function in order to pull the data that pertained to a short period prior to The Great Recession, the period of The Great Recession, and a short period afterward. I attached the periods prior to and afterward in order to have a better understanding the effects of the event on the data. Prior to The Great Recession, all of the commodities seemed to range between 0 and 5,000 USD. However, nickel was trending towards 60,000 USD, which indicates the high volatility and bullish momentum of nickel. During the Great Recession, we see a gradual, yet significant drop in the price of nickel from nearly 60,000 USD to just above 10,000 USD. Despite the outlying nature of nickel from the other metals, all the metals seemed to have suffered adverse effects from various recessionary activities in the metals market. According to supply and demand theory, a determinant of the price of an item is the level of demand for it. If the demand of an item decreases, a frequent activity of firms is to lower the price so as to make the item more attractive to buyers. Given that The Great Recession hit the global economy in a myriad of ways, this understanding may account for the lowering of price during that period.

Softs Sector
I performed the same process with the Softs sector.  I pulled all 3 commodities from the main dataframe and created a separate one, ran the .agg function, used .loc to zoom in the Invasion of Iraq timeline.  I plotted the daily data over this time period, along with the 22-year mean.  For the most part, Softs stayed on or below average during the first 6 years of this time period.  They steadily increased and went above the 22-year mean for the last part of this timeframe.  In 2010, coffee spiked due to poor crop harvest in Colombia.  Cotton also spiked during that time due to shortages resulting from unfavorable growing weather.  Sugar stayed pretty steady during this time period, and only began slightly increasing in 2009, after the 2008 Recession.

Agriculture Sector
For the agriculture sector, I grabbed all relevant commodities from the main data frame and created a new one containing just these.  From there, I ran the aggregate function to get the mean, median, variance, standard error, and standard deviation.  I used the .loc[] function to bring out the dates in the respected event I was analyzing(COVID-19).  From there I was able to plot the data as a line graph to see trends in prices, and how the COVID-19 pandemic may have affected these commodities.  I plotted the mean lines of each of these commodity for the overall 22 years of data as well, to show how skewed prices began to get once the pandemic came into effect. 

Much to my surprise, I can confidently say that the livestock commodities (lean hogs and live cattle), and soybean oil prices had no response to the COVID-19 pandemic.  Corn, soybean meal, wheat, and HRW wheat’s prices were also relatively steady throughout the pandemic with slight dips and spikes along the way, which can be attributed to normal ebbs and flows of the market.  The only commodity of the agriculture industry that showed any significant response to the pandemic was soybean oil.  It was largely affected by COVID-19 and saw drastic rises for the majority of the time, right until things started to fizzle out. 
