## Analysis with Symbology(styling)

- we could analysis Geospatia data with styling e.g 
  - Let's say we have a **data point** of **Earth Quakes** all round the would
  - We could determine the top 10 Event with the highest amount death if the data is provided in the attribute
  - Extract this Top 10 Event and Extract is as a new Layer
  - In the new Layer, we could symbolobize each of the 10 points relatively big according to their size

## HOW TO DO THIS
- Right click on the extracted layer, hoover on **styles** and click **edit symbols** or click on the **icon open layer styling**
- In the **symbol selector** click on the **icon** that says **data defined overide** which is opposite of **size** and click on **Assistant**
- Select the **source** from the table which we wanna use e.g total_death
- Then click on the infinity button that says (**fetch value range from layer**)
- click okay and then click okay
- This will display the 10 points where earthquake has the highest amount death relative to the size of the point
**NOTE:**
- After selecting our **source** and **fetch value range from layer**
- It will generate **Value from** and **Value TO** based on the value of the death of each of the 10 point
- We could manually change the range of the value e.g lets say the Top 10 ranges from 43202 - 7600000, we could choose to manually change it to be from 5000.000000 to 80000.00000



## Adding a legend

- on the **select symbol** click on `marker` and navigate to `Advanced` and click on it
- select **Data defined size legend**
- and pick btw **seperated legend items** or **colapse legend**