# homework-3
Code use in homework of Data Engineer Zoomcamp 2024


### Q 1
```
SELECT COUNT (DISTINCT pulocationid)
FROM `green_taxi.green_taxi`;
```

### Q3
```
SELECT COUNT ( fare_amount )
FROM `green_taxi.green_taxi`
WHERE fare_amount = 0;
```


### Q4
```
CREATE OR REPLACE TABLE green_taxi.green_cluster
CLUSTER BY lpep_pickup_datetime, PULocationID  AS
SELECT * FROM `green_taxi.green_taxi`;
```
