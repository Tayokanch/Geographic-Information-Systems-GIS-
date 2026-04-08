# 🗺️ Data Normalisation in GIS (Beginner Notes)

## 📌 Definition
Data normalisation is the process of converting raw data into a standardised form so different areas can be compared fairly.

---

## 🎯 Why it’s Important
- Raw data can be misleading (e.g., larger areas often have larger values)
- Enables fair comparison between different locations
- Improves accuracy in maps and spatial analysis
- Prevents incorrect conclusions

---

## 🔧 Common Methods
- **Per Area**  
  Population ÷ Area = Population Density (people/km²)

- **Per Capita**  
  e.g., Crimes per 1,000 people

- **Percentages**  
  e.g., % of land used for residential purposes

- **Scaling**  
  - Min-Max (0–1 range)  
  - Z-score (distance from mean)

---

## 📊 Example
- Area A: 50,000 people / 100 km² = 500 people/km²  
- Area B: 10,000 people / 10 km² = 1,000 people/km²  

👉 Area B is more densely populated despite having fewer people.

---

## 🧰 In QGIS
- Use **Field Calculator** or **Refactor Fields**
- Example formula: "Population" / "Area"
- Calculate `Density`
  - Population / Land Area
- Calculate `rate`
    - COVID19 cases / Population
    - Unemployed persons / total working-age population
