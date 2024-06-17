# 3A
## Taxi Data
2023 Taxi data download from here: https://data.cityofchicago.org/Transportation/Taxi-Trips-2023/e55j-2ewb/data 

After downloading data: 
1. install xsv package in your local machine:
View:https://brew.sh/
View:https://formulae.brew.sh/formula/xsv

2. run in Terminal to select the wanted columns, and name the new file as cleaned_taxi_trips.csv
```
xsv select "Trip Start Timestamp,Trip End Timestamp,Trip Seconds,Trip Miles,Pickup Community Area,Dropoff Community Area,Fare,Tips,Tolls,Extras,Trip Total,Payment Type,Pickup Centroid Latitude,Pickup Centroid Longitude,Dropoff Centroid Latitude,Dropoff Centroid Longitude" Taxi_Trips_-_2023.csv > cleaned_taxi_trips.csv
```
This makes the dataset down to around 950mb, for certain analysis, you can select your target columns with the same approach.

## Weather Data
