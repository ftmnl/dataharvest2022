# dataharvest2022

# Exercise

Goal: Map all coal power plants and their energy output in your country and compare, if possible, 2013 with 2019, or use another date range.

Steps:
1. Data is from Resource Watch and the US census bureau. You can find the data [here](https://github.com/ftmnl/dataharvest2022/blob/main/data/dataharvest.zip) .
2. Import csv with the QGIS Data Source Manager (button with three squares in red, yellow and blue) and use lat and lon columns to make your data spatial.
3. Filter powerplants by GWh in 2013 and 2019. Right click on coal plant layer, use filter and enter this code "generated_gwh_2013" != 'NULL' AND "generated_gwh_2019" != 'NULL'.
4. Create a new column in the attributes table (right click on coal plant layer) with the field calculator. Enter a new colunm name, data type (real/decimal) and substract the 2019 column from the 2013 column.
5. Join the results of the calculation from the previous step with the shapefile of US states and calculate the mean of the generated output, using Join attributes by location (summary)
6. Classify the data (right click on the new joined layer, properties, control feature symbology), choose graduate symbols at the top, classify and make a choropleth map)
