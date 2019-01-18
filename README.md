# Client Project: Estimating Income at Risk Following Disaster Events

#### Shawn Mitchell
#### Brandon Miranda
#### Guillaume Manderscheid


### Executive Summary

This project displays potential income losses for a region within a state, selected by the user on a map.  Additional state-wide information on occupation employment numbers and average wages per occupation are also provided.

### Libraries Required
pandas<br>
numpy<br>
json<br>
plotly<br>
ipywidgets


### Data Dictionary<br>
Data dictionary : dataframe 1 : zipcode summary statistics<br>
Affected ZIP Codes : zipcodes<br>
Yearly Estimated Income Risk : total yearly income of the given zipcode<br>
Population : population of the zipcode<br>
City : city containing the zipcode<br>
County : county containing the zipcode (zipcodes can belong to two counties)<br>
dataframe 2 : summary industry sectors for the selected state<br>
Occupation : 20 different occupations regrouping all essential economic industries in the US<br>
Total employment : number of employees in the state and in each sector<br>
Average hourly rate : How much is an hour of work worth in this state on average and for each occupation<br>
Average annual salary : How much is a year of work worth in this state on average and for each occupation<br>
10th - 25th - median - 75th - 90th percentiles : segmentation of incomes, to compare with other states


### Code Source References

https://plot.ly/~empet/14692/mapbox-choropleth-that-works-with-plotly/#/<br>
https://plot.ly/python/selection-events/
