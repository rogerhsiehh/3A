# 3A
## Taxi Data
2023 Taxi data download from here: https://data.cityofchicago.org/Transportation/Taxi-Trips-2023/e55j-2ewb/data 
## All Data
If you download this same data folder to the same folder where you have the other file, you should be able to run everything.
Link to the data folder:
https://drive.google.com/drive/folders/1ftWG1p_dhvVbv6A6tXcc0b_EZV4tw-z6?usp=drive_link

For example, the below code need to access csv file from data folder:
To-do: go to the google drive link, download the data folder and put it into the same jupyter notebook file.
```python

census_tract_daily = pd.read_csv("data/census_tract_daily_data.csv")
