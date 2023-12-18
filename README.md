<img src="http://imgur.com/1ZcRyrc.png" style="float: left; margin: 20px; height: 55px">

# Project 1: Data Analysis of Singapore's Rainfall And Its' Influence On Dengue Cases



<br>

<h4> * As part of our data course, we were required to create a project based on Singapore's weather data, including creating our own problem statement. *</h4>

    
## Background
---

Singapore's climate does not vary much from month to month, and there are no distinct wet or dry seasons.<sup>[1](http://www.weather.gov.sg/climate-climate-of-singapore/#:~:text=Singapore%20is%20situated%20near%20the,month%2Dto%2Dmonth%20variation)</sup> However, a higher rainfall occurs during the two monsoon seasons from November to January and June to September.

Its' metrics such as temperature, humidity, sunshine, and rainfall etc. have been recorded by the government at the Changi climate station.

Dengue fever (DF) and dengue hemorrhagic fever (DHF) are endemic diseases in many regions. Transmission of the virus is made through the female *Aedes aegypti* mosquito.<sup>[2](https://www.who.int/news-room/fact-sheets/detail/dengue-and-severe-dengue)</sup>

Singapore, along with many other tropical countries, take the brunt of the dengue virus<sup>[3](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3373041/)</sup> due to the countries' climates being ideal breeding grounds for Aedes aegypti. DF and DHF is an increasing concern for many in Singapore, especially during the Covid-19 pandemic period.<sup>[4](https://www.straitstimes.com/singapore/health/more-people-have-died-from-dengue-than-from-covid-19-in-singapore-this-year)</sup> As dengue cases are on the rise, it is important to look at how the spread of the disease can be minimised.


### Problem Statement

As such, we want to predict future dengue cases using the weather data in Singapore so appropriate measures can be put in place to minimise the number of dengue cases.



## Data Dictionary
----

*weather_disease_monthly_data.csv*

|Feature|Type|Datasource|Description|
|---|---|---|---|
|dengue_fever_cases|integer|weekly-infectious-disease-bulletin-cases|Number of recorded cases of Dengue Fever in an epidemiological week|
|dhf_cases|integer|weekly-infectious-disease-bulletin-cases|Number of recorded cases of Dengue Haemorrhagic Fever in an epidemiological week|
|daily_max_temp|float|monthly_nea_singstat_rain_humidity|The monthly and annual mean daily minimum temperature recorded at the Changi Climate Station|
|daily_min_temp|float|monthly_nea_singstat_rain_humidity|The monthly and annual mean daily maximum temperature recorded at the Changi Climate Station|
|extreme_max_temp|float|monthly_nea_singstat_rain_humidity|The monthly extreme maximum air temperature recorded at the Changi Climate Station|
|extreme_min_temp|float|monthly_nea_singstat_rain_humidity|The absolute extreme minimum air temperature recorded at the Changi Climate Station|
|total_rainfall|float|monthly_nea_singstat_rain_humidity|The total monthly rainfall recorded at the Changi Climate Station|
|total_highest_daily_rainfall|float|monthly_nea_singstat_rain_humidity|The highest daily total rainfall for the month recorded at the Changi Climate Station|
|no_of_rainy_days|float|monthly_nea_singstat_rain_humidity|The number of rain days* in a month recorded at the Changi Climate Station|
|sunshine_daily_mean|float|monthly_nea_singstat_rain_humidity|The monthly mean sunshine hours in a day recorded at the Changi Climate Station|
|min_relative_humidity|float|monthly_nea_singstat_rain_humidity|The absolute extreme minimum relative humidity for the month recorded at the Changi Climate Station|
|mean_daily_humidity|float|monthly_nea_singstat_rain_humidity|The monthly mean relative humidity recorded at the Changi Climate Station|
|monthly_mean_temp|float|monthly_nea_singstat_rain_humidity|The monthly mean air temperature recorded at the Changi Climate Station|

*\* day with rainfall amount of 0.2mm or more*


## Analysis & Conclusions Summary
---

As we explored the trends of dengue and weather in Singapore, we can see that the 2 main weather that could affect dengue trends is temperature, and rainfall.

Based on my exploration on whether we are able to predict future dengue cases using the weather data in Singapore, we can say that there is a small relationship between the temperature and rainfall, and its effects on the number of dengue cases.

However, as we have seen throughout this exploration, the relationship is not extremely strong. More research shows many other factors affecting the number of DF and DHF cases, including changes in serotype as well as the COVID-19 pandemic, and the preventive measures put in place by the government. Therefore it cannot be completely predicted only using weather data in Singapore

## Sources
---
### Data Sources

* [Singapore's Monthly Weather Data – singstat.gov.sg](https://tablebuilder.singstat.gov.sg/table/TS/M890081)
* [Singapore's Weekly Infectious Diseases – data.gov.sg](https://data.gov.sg/dataset/weekly-infectious-disease-bulletin-cases)

### Research Sources

[1] [Meteorological Service Singapore](http://www.weather.gov.sg/climate-climate-of-singapore/#:~:text=Singapore%20is%20situated%20near%20the,month%2Dto%2Dmonth%20variation) <br/>
[2] [World Health Organization](https://www.who.int/news-room/fact-sheets/detail/dengue-and-severe-dengue) <br/>
[3] [Dengue Prevention and 35 Years of Vector Control in Singapore](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3373041/) <br/>
[4] [2020 Covid and Dengue Rise](https://www.straitstimes.com/singapore/health/more-people-have-died-from-dengue-than-from-covid-19-in-singapore-this-year) <br/>
[5] [2021 Highest Dengue Cases In 4 Months](https://www.straitstimes.com/singapore/dengue-cases-cross-6000-mark-in-less-than-4-months-exceeding-whole-of-2021) <br/>
[6] [National Centre for Infectious Diseases](https://www.ncid.sg/Health-Professionals/Articles/Pages/Epidemic-Dengue-in-Singapore-During-COVID-19-Pandemic.aspx) <br/>
[7] [Effects of Temperature and Heatwaves on Dengue in Singapore](https://www.sciencedirect.com/science/article/pii/S0048969721001832#:~:text=Studies%20have%20shown%20that%20an,et%20al.%2C%202009)<br/>
[8] [Highest Dengue Death Tolls](https://www.straitstimes.com/singapore/health/singapore-records-19-dengue-deaths-in-2022-nearly-four-times-2021-s-toll)