## Graduation symbology in GIS

`Graduated symbology `is used to visualize numeric (continuous) data by grouping values into ranges (classes) and applying a gradual change in symbol (e.g. color or size).

**When to Use:** Use this when your data answers:
“How much?” or “How big?”

Examples:

- Tree height
- Population
- Elevation
- Temperature

**How It Works**

- Select a numeric field (e.g. height)
- Divide values into ranges (e.g. 0–5, 5–10, 10–15)
- Apply a color ramp or size variation

**🌳 Example (Tree Heights)**

| Height Range | Class  | Color       |
| ------------ | ------ | ----------- |
| 0–5m         | Small  | Light Green |
| 5–10m        | Medium | Green       |
| 10–20m       | Tall   | Dark Green  |


**✅ Key Points**
- Works only with numeric data
- Shows magnitude or intensity
- Helps identify patterns and distribution


## How Apply Graduation Symbology QGIS

- right click on the layer(data) and select `properties`
- change `Single Symbol` to `Graduated`
- Select which value /field of the table we wanna use
- pick a `color ramp`
- select `mode` (Natural break)
- click `classify`
- 