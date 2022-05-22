# dataharvest2022

## Exercise

Goal: Map all coal power plants and their energy output in the US and show the difference in output between 2013 and 2019 on a choropleth map.

### Steps:
1. Download the data [here](https://github.com/ftmnl/dataharvest2022/blob/main/data/dataharvest.zip) (right click on link: save as..). Unzip the file in a convenient location on your computer. 
2. Import the csv file (coal plants data) with the QGIS Data Source Manager (button at the top with three squares in red, yellow and blue) and use latitude and longitude columns to make your data spatial.
3. Filter powerplants by GWh in 2013 and 2019. Right click on coal plant layer, use filter and enter this code "generation_gwh_2013" != 'NULL' AND "generation_gwh_2019" != 'NULL'. Press 'test' to see if your query is correct. If so, proceed.
4. Create a new column in the attributes table (right click on coal plant layer) with the field calculator (abacus icon). Enter a new colunm name (e.g. difference_2013_2019), data type (real/decimal) and substract the 2019 column from the 2013 column ("generation_gwh_2013" - "generation_gwh_2019").
5. Join the results of the calculation from the previous step with the shapefile of US states and calculate the mean of the generated output, using Join attributes by location (summary). 
6. Classify the data (right click on the new joined layer, properties, control feature symbology), choose graduate symbols at the top, classify and make a choropleth map)
