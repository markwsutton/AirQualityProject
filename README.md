# AirQualityProject

We began with the question, “How have COVID-19 lockdowns impacted pollution?”

After looking at several other potential proxies for pollution (waste, energy use, and water) we settled on using the Air Quality Index (AQI). The AQI was clearly the best data set to use, as it is global and measured multiple times a day. We pulled our data from the Air Quality Open Data Platform.
    
Research questions:
    1)  What is the best way to measure air quality and how it changed during COVID-19 lockdowns?
    2)  Which of the cities examined show the largest and least reduction in PM2.5 during COVID-19 lockdown dates?
    3)  Looking at different types of pollutants (PM2.5 vs. O3) -- are the patterns consistent, or not, for each city?
    4)  Were there any other major events or factors that influenced air quality during the time period studied?

Methodology
    1)	Selected nine cities that we thought would tell an interesting story given the dynamics of pollution/COVID-19 policies
        	New York, LA, Houston, Jacksonville, Shanghai, Beijing, Wuhan, New Delhi
    2)	First we downloaded CSV files from the open data platform
    3)	In addition to 2020 data we took data from the past three years in order to create a baseline
    4)	We cleaned the data, removing extraneous information from CSVs and selecting for O3 and PM2.5
        	We used PM2.5 and O3 because of the five pollutants captured in the AQI, they are the most frequently measured and have the most data       associated with them
        	Since countries don’t all use the same index, and because the AQI is not a linear measurement of pollutants, we had to reverse engineer the scores into units of measurement for O3 and PM2.5
    o	Merged the average medians of past three years to create a baseline to compare against


Insights and Observations
    1)	AQI is not a linearly related to measurements
    2)	Data suggests that cities major lock down had more reduction of PM2.5, and cities with less strict lockdown had no change or even increases 
    3)	The correlation of PM2.5 vs O3 is inverse -- more sun actually increases O3 production because it is a secondary pollutant
    4)	Other important factors included the Saharan Dust Storm which reached both Houston and Jacksonville, spiking their PM2.5 levels


