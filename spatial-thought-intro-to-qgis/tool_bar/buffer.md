## 🟢 Buffer in QGIS

**Buffer** creates a zone around **points, lines, or polygons** at a specified distance.

---

### 🔹 Function:
- Generates a new layer showing areas within a given distance from features.
- Distance is measured in the **layer’s CRS units** (meters for projected CRS, degrees for geographic CRS).

---

### 🔹 Common Use Cases:
1. **Environmental analysis:**  
   - Create a 500m buffer around rivers to identify flood risk zones.  
2. **Urban planning:**  
   - Find buildings within 200m of a proposed road.  
3. **Access analysis:**  
   - Identify areas within walking distance of bus stops.

---

## 🔵 Dissolve Result Option

When creating a buffer, the **“Dissolve result”** checkbox determines how overlapping buffers are handled.

### 🔹 Behavior:
- **Checked:** Overlapping buffers are **merged** into a single polygon.  
- **Unchecked:** Each feature’s buffer remains **separate**, even if they overlap.

---

### 🔹 Example:

You have 3 nearby schools and create a 500m buffer around each:

| Dissolve Result | Appearance | Use Case |
|-----------------|-----------|----------|
| Unchecked       | 3 separate overlapping circles | Analyze per-school coverage |
| Checked         | 1 merged polygon showing total coverage | Analyze overall area coverage |

---

### ⚠️ Important Notes:
- Ensure your layer is in a **metric CRS** (e.g., meters) for accurate distances.  
- Use **dissolve** when total coverage matters; leave unchecked for per-feature analysis.

---

### 🧠 Tip:
- For UK data: Reproject to **EPSG:27700 (British National Grid)** before buffering to avoid errors in distance calculations.