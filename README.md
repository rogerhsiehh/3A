# 3A
## Taxi Data
2023 Taxi data download from here: https://data.cityofchicago.org/Transportation/Taxi-Trips-2023/e55j-2ewb/data 
## Columns in original dataset
Trip ID 	Taxi ID 	Trip Start Timestamp 	Trip End Timestamp 	Trip Seconds  Trip Miles 	Pickup Census Tract 	Dropoff Census Tract 	
Pickup Community Area 	Dropoff Community Area 	Fare  Tips 	Tolls 	Extras 	Trip Total 	Payment Type 	Company 	Pickup Centroid Latitude 	
Pickup Centroid Longitude 	Pickup Centroid Location   Dropoff Centroid Latitude 	Dropoff Centroid Longitude 	Dropoff Centroid Location

### Some descriptions:

|Variable|Description|
|----|------|
|Community Areas|The city of Chicago is divided into 77 community areas. An area often corresponds to a neighborhood or encompasses several neighborhoods, but the areas do not always correspond to popular conceptions of the neighborhoods. The dataset has all 77 areas|
|Census Tracts|The U.S. Census uses different geography areas for it's collection purposes. Census tracts are small areas of about 1200 households, or 2000-4000 people. The are 866 Chicago census tracts. The dataset has up to 798 census tracts included|


After downloading data: 
1. install xsv package in your local machine:
View:https://brew.sh/
View:https://formulae.brew.sh/formula/xsv

2. run in Terminal to select the wanted columns, and name the new file as cleaned_taxi_trips.csv
```
xsv select "Trip Start Timestamp,Trip End Timestamp,Trip Seconds,Trip Miles,Pickup Census Tract,Dropoff Census Tract,Pickup Community Area,Dropoff Community Area,Fare,Tips,Tolls,Extras,Trip Total,Payment Type,Pickup Centroid Latitude,Pickup Centroid Longitude,Dropoff Centroid Latitude,Dropoff Centroid Longitude" Taxi_Trips_-_2023.csv > cleaned_taxi_trips.csv
```
This makes the dataset down to around 950mb, for certain analysis, you can select your target columns with the same approach.

To download the cleaned_taxi_trips.csv file, check here: https://drive.google.com/drive/folders/1ftWG1p_dhvVbv6A6tXcc0b_EZV4tw-z6?usp=drive_link
