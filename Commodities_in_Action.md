Commodities in Action
    by:  Rebecca Davidson, Chibuzor Ejiaga, & Dylan McGullan


For this project, we chose to focus on commodities and how different historical events have impacted those commodity prices.  We pulled a dataset from kaggle.com that contained commodity prices from early 2000 to late 2022.  We looked at the data as a whole, then divied up the workload by sector and by historical event.  The breakdown is the following
    Rebecca:    Energy Commodities during the Invasion of Iraq in 2003-2011
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

We cleaned up the original dataset, replacing empty cells with 0, and formatting the date column as the index.  We also converted the prices from EUR to USD by using a 1.09 conversion rate.  During the data cleaning process, we discovered the gasoline prices between the years 2000 to 2005 were missing and we replaced them with 0.  We are aware that would skew the data.  We also discovered that several of these commodity price values were amplified by a factor of 100. Soybeans, corn, ULS diesel, wheat, gasoline, and coffee were all off by roughly a factor of 100.  Instead of changing the dataset by dividing those values by 100 or dropping those commodities altogether, we decided to still use the data because while the values were off, the data would would still represent a realistic trend. 

Our first visual is a graph showing all prices for all commodities for the years 2000-2022.  The three historical events we are focusing on are annotated on the plot.  The first takeaway from the plot is that nickel sits way higher than all the other commodities, making it difficult to see the rest of the data.

After this, we ran the .agg function on the dataset to get the mean, median, variance, standard deviation, and standard error of the mean over the entire 22-year period.  We plotted boxplots on the whole dataset, but it was difficult to analyze the plot because all the commodities are on such a wide range of prices.  From this point, we each focused on our sectors and historical event.

Energy Sector
I pulled all 6 energy commodities from the main dataframe and created a separate dataframe.  I ran the .agg function on it.  Then I used the .loc function to pull data within a date range to focus on the Invasion of Iraq that occurred between 2003-2011.  I plotted this daily data, along with the mean of each over the 22-year period.  This would show how the daily data over this specific time period compared to the 22-year mean.  During the Invasion of Iraq, energy commodities generally had an upward trend.  The 2008 Recession did occur during this time period also, but on average, the trend was in the positive direction and much of it sat above the 22-year mean.

Softs Sector
I performed the same process with the Softs sector.  I pulled all 3 commodities from the main dataframe and created a separate one, ran the .agg function, used .loc to zoom in the Invasion of Iraq timeline.  I plotted the daily data over this time period, along with the 22-year mean.  For the most part, Softs stayed on or below average during this time period.  In 2010, coffee spiked due to poor crop harvest in Colombia.  Cotton also spiked during that time due to shortages resulting from unfavorable growing weather.  Sugar stayed pretty steady during this time period, and only began slightly increasing in 2009, after the 2008 Recession.