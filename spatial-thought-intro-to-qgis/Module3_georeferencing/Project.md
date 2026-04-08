## Georeferencing Project

- This project is about georeferencing an Old Map of a City Bangalore. Bangalore used to known for a lot of lakes however, due to urbanisation alot of this lake has been lost
- The task here is to `overlay` an Old Map of this City to the Present current state of the City to determine which lakes has been lost due to urbanisation.

## Steps to follow
1. Find a way to georeference the old map of the City so it can overlay exactly on the current map
2. Digitize each of the lakes in the old map and compare it with the current based map 

# This will let use know how a place has changed over time

## Steps to follow
1. Go to `layer` on the Menu Bar, and select `Georeferencer`
2. load the Image using `Open Raster` button
3. Check the old map and compare it to the current map (OSM), figure any on the **current map (OSM)** that still exist on the **Old Map**
4. on the **Old Map**(image) loaded on `Georeferencer menu`, click the tool called **Add GCP Point** and click on any corner of the **common feature** that still exist on both maps
   - This will pop up a **Menu bar**, then select **From Map Canvas**
   - GO OSM map, then click on the same point / corner of the same feature
   - This will automatically generate coordinate for that Feature we selected
5. Repeat step 4 multiple times across the old map to generate as many cordinate as possible.
6. on the `Georeferencer menu`, click on `Transformation setting icon`
7. select `transformation=polynomia2` (The transformation we are picking depends on what we are working on, and the kind of output we wanna get)
8. Select `output file directory and name` then `OK
9. Click on the Play button to start the Georefercing, and once done, Go to the OSM layer.
10. The Old Map will now be overlayed on the current map (OSM)
