# Air Quality

We began with the question, “How have COVID-19 lockdowns impacted pollution?”

After looking at several other potential proxies for pollution (waste, energy use, and water) we settled on using the Air Quality Index (AQI). The AQI was clearly the best data set to use, as it is global and measured multiple times a day. We pulled our data from the Air Quality Open Data Platform's Worldwide COVID-19 dataset:  
https://aqicn.org/data-platform/covid19/
    
**Research questions:**  
    1)  What is the best way to measure air quality and how it changed during COVID-19 lockdowns?  
    2)  Which of the cities examined show the largest and least reduction in PM2.5 during COVID-19 lockdown dates?  
    3)  Looking at different types of pollutants (PM2.5 vs. O3) -- are the patterns consistent, or not, for each city?  
    4)  Were there any other major events or factors that influenced air quality during the time period studied?  

**Methodology:**  
    1)	Selected eight cities that we thought would tell an interesting story given the dynamics of pollution/COVID-19 policies  
        - New York, LA, Houston, Jacksonville, Shanghai, Beijing, Wuhan, New Delhi  
    2)	First we downloaded 7 CSV files from the open data platform  
    3)	In addition to 2020 data we took data from the past three years in order to create a baseline  
    4)	We cleaned the data, removing extraneous information from CSVs and selecting for O3 and PM2.5  
        - We used PM2.5 and O3 because of the five pollutants captured in the AQI, they are the most frequently measured and have the most data associated with them  
        - Because the AQI is not a linear measurement of pollutants, we chose to convert the scores into units of measurement for O3 and PM2.5  
        - We looked at lockdown dates in each of the 8 cities  
    5)	Merged the average medians of past three years to create a baseline to compare against  


**Insights and Observations:**   
    1)	AQI is not a linearly related to measurements  
    2)	Wuhan and New Delhi had the largest reductions in air pollution, and Houston and Jacksonville had the least reductions (actually increases) in air pollution   
    3)	The correlation of PM2.5 vs O3 is inverse -- more sun actually increases O3 production because it is a secondary pollutant  
    4)	Other important factors included the Saharan Dust Storm which reached both Houston and Jacksonville, spiking their PM2.5 levels  

**File and folder structure:**  
    1) On the top level, we have our presentation, analysis files, and a Resources, outputs and Datacleaning folders  
        - Resources includes the CSV files we outputted from datacleaning, and other data that we found in our analyses and used for graphs    
        - One Jupyter Notebook for each city, and another general analysis file  
        - The PDF of our final presentation  
    2) Within Datacleaning, we have the Jupyter Notebooks that show the datacleaning, the conversion of data from index, and the output CSVs for each year
    
Images from presentation:    

![Image](https://github.com/markwsutton/Citibike-Analysis-Tableau/blob/main/images/1-AQI.png)
![Image](https://github.com/markwsutton/Citibike-Analysis-Tableau/blob/main/images/2a-AQI.png)
![Image](https://github.com/markwsutton/Citibike-Analysis-Tableau/blob/main/images/3-AQI.png)
![Image](https://github.com/markwsutton/Citibike-Analysis-Tableau/blob/main/images/4-AQI.png)
