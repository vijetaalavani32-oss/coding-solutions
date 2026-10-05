# Weather Observation Station 5

![Difficulty](https://img.shields.io/badge/Difficulty-Medium-yellow)

## Problem

Query the list of *CITY* names starting with vowels (i.e., `a`, `e`, `i`, `o`, or `u`) from **STATION**. Your result *cannot* contain duplicates.

**Input Format**

The **STATION** table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" title="Station.jpg" />

where *LAT\_N* is the northern latitude and *LONG\_W* is the western longitude.

**Constraints**

 

**Output Format**

## Solution

**Language:** db2  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-05T11:34:04.628Z  

```db2
SELECT CITY, LENGTH(CITY)
FROM STATION
ORDER BY LENGTH(CITY), CITY
FETCH FIRST 1 ROW ONLY;
SELECT CITY, LENGTH(CITY)
FROM STATION
ORDER BY LENGTH(CITY) DESC, CITY
FETCH FIRST 1 ROW ONLY;

```

---

[View on HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-6/problem)