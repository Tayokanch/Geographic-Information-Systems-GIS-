## JOINS

`Joins`: This is used for data merging in GIS. Its also a Techniques for Merging data from 2 separate layers in GIS

**METHOD OF JOINS**

- `Table Joins`: This is used when want to join `one vector spatial data` and some `tabular data` together to create some data set for mapping. 
**Example**: lets say we have 2 datasets
  1. we have shapefile of all countries with an attribute called **"name"** containing the name of the country
  2. We also have an Excel file with 2 columns A **"country"** and **"GDP"**
  - we could use this datas to create a dataset of **gdp_per_capital**
  - In QGIS **Table joins** is performed in the **Attribute Table** using Join Attribute by Field Value
  
- `Spatial Joins`: This is used to join `two vector dataset` based on their common spatial attributes or relationships  to create a new dataset
  **Example 1:**
  - We have a Point layer of **'cities'**
  - we have a polygon layer of **'states'**
  - We could perform a spatial join by joining both datasets by to display which `state` each `cities` belongs to or located.
  
  **Example 2**:
  - We haave a point Layer of 'earthquakes'
  - We have a Point Layer of 'populated places'
  - We could determine the nearest populated place for each earthquake USING the **JOIN Attribute by Nearest**


- `Raster Sampling`: This is used when we have `rasta data` e.g **an elevation data** and some **polygon or point** that we want to extract information from the `Rasta data ` using vector data(point, line, or polygon)

  **Example1**:
  - We have a Polygon Layer of a "river basin"
  - We have a Raster layer of "rainfall"
  - We could calculate the average rainfall in each basin. This analysis is called **Zonal Statistics** in GIS

  **Example2**:
  -  We have a Point layer of **'cities'**
  - We have a Raster layer of 'Maximum Temperature'
  - We could Determine the Maxiumum Temperature of each **'cities'**. This could be done using the Tool called **Raster Sampling** in QGIS

There are 3 different Tools in QGIS for **Sampling Raster Data**
1. Zonal Statistics
2. Same Raster Values
3. Drape (Set Z values from Raster)

  
