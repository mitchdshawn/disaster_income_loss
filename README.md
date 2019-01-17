# Client Project: Estimating Income at Risk Following Disaster Events

#### Shawn Mitchell
#### Brandon Miranda
#### Guillaume Manderscheid


### Executive Summary

This project displays potential income losses for a region within a state, selected by the user on a map.  Additional state-wide information on occupation employment numbers and average wages per occupation are also provided.

### Libraries Required
pandas
numpy
json
plotly
ipywidgets


### Data Dictionary
Data dictionary : dataframe 1 : zipcode summary statistics
Affected ZIP Codes : zipcodes
Yearly Estimated Income Risk : total yearly income of the given zipcode
Population : population of the zipcode
City : city containing the zipcode
County : county containing the zipcode (zipcodes can belong to two counties)
dataframe 2 : summary industry sectors for the selected state
Occupation : 20 different occupations regrouping all essential economic industries in the US
Total employment : number of employees in the state and in each sector
Average hourly rate : How much is an hour of work worth in this state on average and for each occupation
Average annual salary : How much is a year of work worth in this state on average and for each occupation
10th - 25th - median - 75th - 90th percentiles : segmentation of incomes, to compare with other states


### Code Source References

https://plot.ly/~empet/14692/mapbox-choropleth-that-works-with-plotly/#/
https://plot.ly/python/selection-events/
