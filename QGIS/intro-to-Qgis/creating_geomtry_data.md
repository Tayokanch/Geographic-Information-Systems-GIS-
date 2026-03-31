## HOW TO CREATE A GEOMETRY(POINT, LINE , POLYGON) DATA in QGIS

- Click `Layer` from the **TOP MENU**
- SELECT `Create Layer` and Click on `New Shapefile Layer`
- select the prefered `directory`, `filename`, `geometry type` , create a field by adding `field name & and type if needed to the TABLE and add the this field.` then create this later
- once the layer is created we can start creating the gemoetry data by:
  - Select the layer we want edit, right click and select `Toggle Editing`
  - select `vertex tool` from the menu
  - on the Dashboard click on `add polygon` or `add line` depending on the Geometry we are working on
  - Navigate the cursor to the shape(building) we want to create and once created, right click to fill the information(`id: 1` & and `fieldname: Etihad Stadium`) of the created shape(id, name) based on the table we have when creating the layer


## How to Print out a Map
- After creating the Geometries and we want to convert it to a real map 
  - Navigate to the `TOP Menu` dropdown, click on `project` and select `New Print Layout`
  - Give the Print Layout a `name` and click ok.
  - you will be navigae to a new dashboard to creat this `Print Layout Map`
  - In this **new dashboard** click on `add map`, then us the cursor to create a rectangular shape on the while layout on the new Dashboad, this will automatically render our map on the print layout.
   - This is where we would add `legend` `scale`, `north arrow` etc and save the print as a pdf, svg, etc.