# PySpark Analysis: NYC TLC Trips Records (FHVHV) Data Feb 2021

## Tech Stack
1. PySpark
2. Google BigQuery
3. Google Cloud SDK

## Dataset
[NYC TLC Trips Records (FHVHV)](https://d37ci6vzurychx.cloudfront.net/trip-data/fhvhv_tripdata_2021-02.parquet)

## Problems
1. How many taxi trips were there on February 15?
2. Find the longest trip for each day!
3. Find Top 5 Most frequent `dispatching_base_num`!
4. Find Top 5 Most common location pairs (PUlocationID and DOlocationID)!
5. Write all of the result to BigQuery table!

## Results:
1. |trips_feb15|
   |--|
   |425928|
2. Top ten result:
   |      date|longest_trip|
   |----------|------------|
   |2021-02-01|      212.43|
   |2021-02-02|      282.78|
   |2021-02-03|      184.26|
   |2021-02-04|      203.97|
   |2021-02-05|      245.35|
   |2021-02-06|      275.32|
   |2021-02-07|      216.36|
   |2021-02-08|       253.5|
   |2021-02-09|      480.73|
   |2021-02-10|       512.5|
3. |top5_dispatching_base_num|total_trip|
   |-------------------------|----------|
   |                   B02510|   3233664|
   |                   B02764|    965568|
   |                   B02872|    882689|
   |                   B02875|    685390|
   |                   B02765|    559768| 
4. |PULocationID|DOLocationID|total_trip|
   |------------|------------|----------|
   |          76|          76|     45041|
   |          26|          26|     37329|
   |          39|          39|     28026|
   |          61|          61|     25976|
   |          14|          14|     17934|
 5. <img width="538" alt="Screenshot 2023-03-19 at 15 51 44" src="https://user-images.githubusercontent.com/113230789/226164134-e884799e-cd05-4118-a1a4-9e89d8762d48.png">
