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
 
## Summary

Based on the results above, we reached the conclusion that, given the temperature analysis, the surf and ice cream shop business is sustainable year-round.  However, for a more accurate opinion, it would be necessary also analysing preciptation and data from the station with the highest number of temperature observations, as it tends to be more reliable.

  - Preciptation:  
    results = session.query(Measurement.prcp).\
    filter(extract('month', Measurement.date) == 12).all()
    
  - Highest Obsvervation Station:
    results = session.query(Measurement.tobs).\
    filter(Measurement.station == 'USC00519281').\
    filter(extract('month', Measurement.date) == 12).all()
  
