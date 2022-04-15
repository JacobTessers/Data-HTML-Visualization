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
