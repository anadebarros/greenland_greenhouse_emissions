# greenland_greenhouse_gases

From [Statbank, Statistics Greenland](https://bank.stat.gl/pxweb/en/Greenland/), I created two .csv files: emission of greenhouse gasses in Greenland by sector and time (United Nations Framework Convention on Climate Change (UNFCCC)-approach), as well as average monthly air temperature by measuring, time, weather station and month

The measurement unit typically used for reporting total greenhouse gas emissions from the UNFCCC and its annual inventory on greenhouse gas emissions is metric tons of carbon dioxide equivalent (CO2e). This unit allows for the aggregation of emissions from various greenhouse gases, including CO2, methane (CH4), nitrous oxide (N2O), hydrofluorocarbons (HFCs), perfluorocarbons (PFCs), sulfur hexafluoride (SF6), and others, by converting them into their CO2 equivalent based on their global warming potential (GWP).
The UNFCCC inventory provides a comprehensive assessment of greenhouse gas emissions from various sources within a country's jurisdiction, helping to monitor progress towards emission reduction targets and commitments outlined in international climate agreements.

In this project I started by working with the total net emissions of greenhouse gases from 1990 to 2021 (greenland_greenhouse_emissions_total.ipynb). I calculated the maximum and minimum emissions as well as the rate of change in total emissions over time. I then preformed regression analysis using polynomial fitting to understand if there were any emission trends and if they were significant. Plotted residual and predicted values and calculated R-squared and RMSE values to understand model performance. 
Finally, using this model I attempted to predict greenhouse emissions in Greenland over the next 50 years.

I then proceeded to divide emissions by different sectors, and for each, I analysed several aspects individually. These included emissions over time and the contribution (percentage) of different sources, per sector, for the total number of emissions (greenland_greenhouse_emissions_waste.ipynb, greenland_greenhouse_emissions_industrial.ipynb, greenland_greenhouse_emissions_fuel_combustion.ipynb, greenland_greenhouse_emissions_forest.ipynb, greenland_greenhouse_emissions_agriculture.ipynb).

After analyzing each sector individually, I calculated the percentage of emissions from each source to the total net emissions, and explored correlations between total emissions and sector-wise emissions to understand how changes in one sector may affect overall emissions (sector_comparisons.ipynb). I created a correlation matrix and used hypothesis testing to assess the statistical significance of the strongest correlations.

Finally, I attempted to understand if there was a correlation, or a trend between greenhouse gas emissions and average air temperature throughout the same period of time. For this I used some simple statistics and visualizations and again fitted a polynomial model to  capture potential non-linear relationships between emissions, years, and temperature.


Some interesting sources that may give context to my results:

[NASA finds 2011 ninth-warmest year on record](https://climate.nasa.gov/news/668/nasa-finds-2011-ninth-warmest-year-on-record/)

[Greenland ice sheet may disappear with 1.6°C temperature increase](https://www.airclim.org/acidnews/greenland-ice-sheet-may-disappear-16%C2%B0c-temperature-increase)

[Air Pollution and Its Association with the Greenland Ice Sheet Melt](https://www.mdpi.com/2071-1050/13/1/65)

