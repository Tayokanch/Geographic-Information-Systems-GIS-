## Population Density of NYC

**DATA USED**
1. A polygon dataset of NYC
2. A CSV data set with Population field

**Process**
- A table join was done on with data set to using a common field, to have the **population field** join with the **Polygon Attribute**. Using the **Join Attribute by Field** in the **Processing Toolbox**
  
- To determine the **Population Density**, we perform a calculation  using **field calculator** tool in the **Processing Toolbox** by dividing (Area field / population) with a field name "Density".
- After saving and click run, it will create a **New Layer** with a field/column Density in the attribute Table

**Note:** The unit of area is also important, therefore depending on the data we are working on, we might need to do some conversion to get the `unit` that fit our analysis

Example: In this our `Area field` was in `ft `and we had to convert it to `sqm(m2)` during the density calculation
