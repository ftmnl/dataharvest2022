# dataharvest2022

## Exercise 1

Goal: Find all owners of oil and gas extraction licenses in one of the European seas and export these as a list in csv or excel.

Requirements:
1. Use a WFS service. You can find the right one [here](https://www.emodnet-humanactivities.eu/search-results.php?dataname=Active+Licences). 
2. Stuck? Use the documentation of QGIS or look for other QGIS tutorials. Search for: 'importing WFS service', 'using attribute tables', 'exporting to csv', of course all in the context of QGIS.

## Exercise 2

Goal: Map all coal power plants and their energy output in your country and compare, if possible, 1999 with 2019, or use another date range.

Steps:
1. Data is from Resource Watch. You can find the data (csv) [here](https://github.com/ftmnl/dataharvest2022/tree/main/data/global_power_plant_database_v_1_3).
2. Import csv and use lat and lon columns to make your data spatial.
3. Import country administrative borders geodatabase [here](.
4. Filter (using clip or join) power plants from your country.
5. Filter two years. You can choose to export the csv files and perform your calculation there or use the field calculator provided by QGIS.
6. Map the difference: for instance, re-import the result of the calculation from the previous step. 



