# graces_and_johns

##The data for this notebook comes from BigQuery public data set.

SELECT
  year,
  SUM(number) as Graces
FROM
  `bigquery-public-data.usa_names.usa_1910_current`
WHERE
  name= 'Grace'
GROUP BY
  year
  ORDER BY year;
A similar SQL query retrieved the sum of people named John.


The dashboard can be seen [here](https://jacobtessers.github.io/graces_and_johns)
