## Creating  Vector data in QGIS

**DIGITIZING Vector Data**

- Go to `layer` on the menubar
- click on `Create New Layer` and select `New Geopackage layer`
- Select a **Location and filename**, Select the tye of Vector(point, line, polygon), Its most preferable to select `multiPolygon` `multiline` , Or `Multipoints`
- Give **name** for the field, **Type**, and **Maximum Length**
- Then click `add to fill lists`
- **Note** we can add as many fields as needed
- click `OK`


## How to configure a Field to give pre-defined options as our value

- Configure `Attribute form` by going to the **Layers Panel** and **right click** newly created Layer we are about to **digitized**. select `properties` navigate to `Attribute form` and click on it 
- In the `Attribute form` select the fieldname we want to configure with **value options**, go to **Widget Type**, Click on the drop down Menu and select **Value Map**
- Edit both `value` and `description` table based on option we want to give a particular field
  - E.G lets say we have a field that says **status** and we want to set this field you accept only **true** or **false**
  - we can set `value as 1`, `description true` and `value as 2`, `description false` or more if we want more options
  - Navigate to **contraint** check `Not null` to enforce an object to be given a name after digitising
  - check `enforce not null contraint`: This prevent not having NULL and enforces the column to be filled with on of the options. for the example used here (the ` true or false`)

## How To Start Digitizing a Polygon
- Go to `View` on the Menubar, navigate to `Toolbars`
- Select `Snapping Toolbar` and Click on `Enable Snapping` red magnet button to enable to Snapping toolbar
- Select the pencil `Toggle Editing` , then click `Add polygon` button to start editing
- Use `vertex tool` on the menubar to edit the polygon if needed
- Click on `Save Layer Edits` to save our editing


## How to Edit a Vector(Polygon)
- Use `vertex tool` on the menubar to edit the polygon if needed

## How Digitize Multi-Polygon using  Add Part tool

- When digitizing `Add Part` Tool is used to add a Vector(polygon) to another incase they are being demacated and we dont wanna create a field for them. E.g A river was divided or demacated by a line(bridge) on the map, we could digitised the first half part and use advanted to like `Add Part` to add the second half part of the river to the first half to make a single attribute.

**How to do this**
- Digitise the first half part
- Go to `View`, select `Toolbar`, then click on `Advanced Digitizing Toolbar`
- click on the **first half part** then select  `Add Part` from the `Advanced Digitizing Toolbar` tool menu
- - Click on `Save Layer Edits` to save our editing

## Add Ring tool 
- This is a tool within the `Advanced Digitizing Toolbar`. It is used for adding circle inside a digitized polygon