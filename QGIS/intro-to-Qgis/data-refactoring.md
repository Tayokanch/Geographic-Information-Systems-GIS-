## Data Refactoring in QGIS

- When we are using a CSV in QGIS, QGIS isnt always strict about the CVS data type, mostly times a field that is originally `integer`, `Double`, OR `NULL` would turn to a `TEXT` type making it unusable for a numerically analysis.

- Therefore, the field in the CVS that we wanna use for our analysis / classififcation must be converted to a `Double` or `Float` by using `Refactor Fields` from **Toolbox** 
- Pick the CSV file we are working on, then change the particular field we want to refactor from Text - `Double` or `Float`
- This will automatically created a `Refactor Data`