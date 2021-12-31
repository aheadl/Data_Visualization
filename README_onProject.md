# (Dataset Exploration Title)
## by (Andrea Headley)


## Dataset


The Flights dataset was used for this exploration and visualization project. The dataset has data about flights covered by several airlines across several cities in the US. The data consists of flight arrival and departure details for all commercial flights within the USA, from October 1987 to April 2008. This is a large dataset: there are nearly 120 million records in total, and takes up 1.6 gigabytes of space compressed and 12 gigabytes when uncompressed. The dataset resides at
https://www.transtats.bts.gov/DL_SelectFields.asp?gnoyr_VQ=FGJ&QO_fu146_anzr=b0-gvzr.

I decided to only take a segment of the data, because of its size, so I selected all the data for the December 2019 and December 2020. 
Data was extracted into separate csv files - two main files were created, one with flight data for all geographical locations in December 2019 and the other for December 2020. Since there were some lookup tables that provided descriptions of some of the data, I imported a few more csv files and merged that data into the two main dataframes I created. This is noted further down in this project. The decision to choose these time periods was driven by my curiosity to analyze how the travel industry was affected by the Covid pandemic just before the pandemic and in the height of the pandemic.



## Summary of Findings


My approach to exploration was to determine how carriers and airports performed, particurlay focusing on the types of cancellations and delays and how they impacted the carriers and flights. 

**Frequency of flights:**
I looked at the frequency of flights by the different carriers, with a special interest on the difference in the number of flights taken by them in December 2019 and 2020, and found that overall, there were more flights in 2019 than in 2020, and concluded this was directly as a result of the impact the Covid pandemic had on the airline industry. Also found in both years, South West had the most flights, and Hawaiian air the least, but the other carriers did not maintain the same rank year over year. 
***This will be included in the explanatory data presentation.***

**Frequency of delays and causes:**
 I also explored the **frequency of delays (arrival as well as departure)** amongst the carriers, and other causes of the delays (**weather, security, carrier, late aircraft arrival, national air system**) and as I expanded my exploration, I found that the highest frequency of arrival delays across the US in December 2019 was under 200 minutes long, and in 2020 was between 275 and 300 minutes, and that longer delays were less frequent. In general, the most frequent departure delays for both 2019 and 2020 were between 275 and 300 minutes. 
***A look at the departure delays encountered by carriers  will be included in the explanatory data presentation.***

The **weather related delays** were generally larger in 2020, the most frequent was 15 minutes, and 2 minutes in 2019. Longer weather related delays were less frequent. Also seen was that the length of weather related delays was mostly small across all carriers, but there are outliers which indicate that there were instances when delays were very long.

The highest frequency in **security delays** in December 2020 were reasonably small and just one minute below 2019 (17 minutes). Closer exploration of the correlation with carriers revealed that in 2019 the minimum length of security delays were one for all carriers, but the maximum delays varied across carriers, with SkyWest Airlines having the maximum. In December 2020, the minimum delay was one like 2019, but on average smaller than 2019.

The highest frequency of **late aircraft delays** in December 2019 and 2020 were both 15 minutes. A large percentage of this delay appear to be under 1 hour, mainly ranging between 30 and 60 minutes.

Most of the delays **National Air System delays (NAS)** in December 2019 and 2020 lasted from 1 to 20 minutes, and longer delays were less frequent. 
Correlations with carriers showed that overall the delays ranged from 1 to under 100 minutes, but there are outliers across all carriers, indicating that there were times when delays were excessively long, but less frequent.

**The impacts of these delays on cancellations will be included in the explanatory data presentation.**

The most frequent **carrier related delay** in December 2019 was around 1 minute, and 15 minutes in 2020, respectively.


**Frequency of flights from cities of origin**
Most flights in December 2019 originated from Chicago (ORD), followed by Dallas Forth Worth (DFW), Denver (DEN), Charlotte (CLT) and Los Angeles (LAX). While some of the same airports remained within the top 5 in December 2020, the order changed, with Dallas Forth Worth (DFW) being the most frequent, and Denver (DEN), Charlotte (CLT) following.

Further explorations didn’t show any direct correlation between cancelled flights and security, weather, NAS, arrival and departure delays. However arrival and departure delays correlated with one another, as well as security delay and arrival and departure delays, with some data points indicating that there were some arrival and departure delays not related to security delays. There are indications that NAS delays occurred when there were arrival and departure delays. However, there was not enough information to conclude that there is a direct correlation between NAS and security delays, since there were only a minimum amount of data points to be able to draw any conclusions of their relationship.

**Frequency of flights at destination cities**
In 2019, Chicago (ORD) was the most travelled to destination airport, and the next 4 airports following were Dallas Forth Worth (DFW), Denver (DEN), Charlotte (CLT) and Los Angeles (LAX) - very similar to the findings from the analysis of the cities flights originated from. While four of the same airports remained within the top 5 in 2020, the order changed, with Chicago (ORD) falling to 4th place and Dallas Forth Worth (DFW) taking the top spot, followed by Denver (DEN) and Charlotte (CLT). Also in both charts, they have been significant differences in frequency of flights when comparing some airports listed adjacent in the plot. For example, in 2019, there is a big different in frequency of flights at Chicago (ORD) airport, with the number of flights exceeding 25,000 and the lowest under 5000 flights.
***This will be included in the explanatory data presentation.***

**Airports performances by early departures**
I explored the top ten airports with early departures and found that Atlanta airport had the earliest average departure time in both 2019 and 2020, while LaGuardia and SEA Seattle airports were 10th in December 2019 and 2020, respectively.

***This will be included in the explanatory data presentation.***


**Activities at top ten busiest airports**
I explored the top 10 busiest airports (where flights originated) and the volume of the type of cancellations ('Carrier', 'Weather', 'National Air System' and 'Security') to see how they impacted the airports. I found that most cancellations were related to weather in December in 2019 and 2020, and security cancellations only occurred in 2020. In 2019, NAS related cancellations were the least in most airports, except for San Francisco and La Guardia, where delays were significantly higher, and overall, San Francisco airport had the largest combined cancellations.
***This will be included in the explanatory data presentation.***

## Key Insights for Presentation


The key insights that will be presented are :
- The top ten busiest airports
- Departure Performance - Carrier departure times
- Departure and Arrival delays
- Carrier arrival times
- Cancellations and Diversions
- Causes of delays:
- Carrier delays
- Security delays
- Weather delays
- National Air Systems (NAS) delays
- Distribution of flights at origin and destination airports
- Airport performance



