# Project-02

## Goal
How much delay is your flight likely going to have? The goal of this project is to predict flight delay time for a given flight (flight #, date).

## Data Sources
* 2017 Flight delay and cancellation data from [Bureau of Transportation Statistics](https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236)
* 2015 airport volume data scraped from Bureau of Transportation Statistics website: [bts.gov](https://www.transtats.bts.gov/airports.asp?pn=1)
* Historic airport weather data from Iowa State University website: [Iowa State Univerity Mesonet](https://mesonet.agron.iastate.edu/request/download.phtml?network=WA_ASOS)

## Methodology
1. Filter out 2017 flights data to only departing flights that are NOT cancelled and with departure time data
2. Merge airport volume data and weather data with flight data
3. Build linear regression model with the merged flights and airport data to predict flight delay time for a given flight

## Features
1. Airport - # scheduled flights per day for airport where flight departs
2. Flight - MONTH
3. Flight - DAY_OF_MONTH
4. Flight - INBOUND_DELAY: arrival delay from the previous flight for the same aircraft
5. Flight - TURNAROUND_TIME: time between an aircraft's last arrival time to next departure time
6. Flight - Airline
7. Airport weather- wind speed
8. Airport weather- precipitation
9. Airport weather- temperature
