# Surfs Up Analysis
  Analysis of temperature trends in Oahu
  
## Overview of the analysis
Obtain more information about temperature trends before opening the surf shop. Specifically, getting temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round.  The following outputs will be produced:

- Determine the Summary Statistics for June
- Determine the Summary Statistics for December
- A written report for the statistical analysis
  
## Resources
- Data Source: hawaii.sqlite
- Software: Python 3.7.6, Pandas, Jupyter, VSCode, SQLite, SQLAlchemy, Flask

## Results
The analysis of Oahu's weather data data shows that:
  - Average temperature is fairly stable across the year, being June's average slighlyly higher (75 against 71);
  - Temperatures ate more stable whithin the month in June (std 3.26 against 3.75), but both overall fairly stable;
  - Although there are few outliers (56 in December), there are not many cold days, as the 25% percentile is 73 and 69 (with fewer cold days in June)
  
- June Statiscs
![June Statiscs](/June_stats.png)

- December Statiscs
![December Statiscs](/December_stats.png)
  
 -  The total fare in urban cities are signifincatly higher than nom-urbans as shown in the chart below.  But this is mistly explained by higher number of rides, but not as much as total of drivers, as shown in the table above.
 
- Pyber-Fare Summary
![Pyber_fare_summary](/analysis/PyBer_fare_summary.png) 
 
## Summary

Based on the results above, we have the following recommendations:

  - Although there are fewer rides on non urban cities, the number of drivers are not enough to support this demand.  Therefore the company should increase the bumber of drivers in those cities, which by consequence, have a higher compensation per ride.
  - As lower prices per ride ate correlated to higher number of rides, the copany should decrease the price in non-urban areas to increase demand.
  - By reallocating driver's to non-urban areas, there will be room to increase fares on urban cities, and inprove the break-even.
