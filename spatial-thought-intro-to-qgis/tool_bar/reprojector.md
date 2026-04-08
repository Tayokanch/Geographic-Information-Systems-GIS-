# Reprojection in QGIS

## 1. On-the-Fly Reprojection
- Automatically applied for **map display**
- Allows layers with different CRS to **align visually**
- **Does NOT change the original data**
- Controlled by the **Project CRS**

#### ✅ Use Case Example
You load:
- A world dataset in **WGS84 (EPSG:4326)**
- A UK boundary dataset in **British National Grid (EPSG:27700)**

➡️ QGIS displays them aligned using on-the-fly reprojection  
➡️ However, the underlying data remains in different CRS

#### ⚠️ Important
- Only for visualization  
- Not suitable for measurements or analysis  


## 🧭 Enabling On-the-Fly Reprojection in QGIS

On-the-fly reprojection allows QGIS to automatically align layers with different Coordinate Reference Systems (CRS) for **visualization purposes only**.

---

### ✅ Method 1: Enable from Status Bar (Quick Method)

1. Look at the **bottom-right corner** of QGIS
2. You will see the **Project CRS** (e.g. EPSG:4326 or EPSG:27700)
3. Click on it
4. In the window that opens:
   - Set your desired CRS
   - Ensure reprojection is enabled

➡️ QGIS will now automatically reproject all loaded layers to match the project CRS

---

### ✅ Method 2: Enable via Project Properties

1. Go to:
   - `Project` → `Properties`
2. Click on the **CRS** tab
3. Search and select your desired CRS
4. Click **Apply** → **OK**

➡️ This sets the CRS for the entire project and activates on-the-fly reprojection

---

### 🧪 Example

You load:
- A shapefile in **WGS84 (EPSG:4326)**
- Another in **British National Grid (EPSG:27700)**

#### Without on-the-fly:
- Layers appear **misaligned**

#### With on-the-fly:
- Layers **align correctly on the map**
- No changes are made to the original data

---

### ⚠️ Important Notes

- On-the-fly reprojection:
  - ✅ Good for visualization
  - ❌ Not suitable for analysis (distance, area, etc.)

- Always use **Reproject Layer** when:
  - Performing calculations
  - Standardizing datasets

---

### 🧠 Tip

If your layers look “correct” but analysis gives wrong results:
➡️ You are likely relying on on-the-fly reprojection instead of properly reprojecting your data

---

## 2. Reproject Layer (Processing Toolbox)
- Found in **Processing Toolbox → Reproject Layer**
- Performs a **permanent CRS transformation**
- Creates a **new output layer**
- Original data remains unchanged  

#### ✅ Use Case Example
You want to calculate **population density** for UK regions:
- Your dataset is in **WGS84 (degrees)** ❌  
- You reproject to **British National Grid (meters)** ✅  

➡️ Now area calculations are accurate  
➡️ Density results are reliable  

#### ⚠️ Important
- Required for:
  - Distance calculations  
  - Area calculations  
  - Buffering and spatial analysis  

---

## 🔁 Quick Comparison

| Feature                  | On-the-Fly Reprojection | Reproject Layer |
|--------------------------|------------------------|------------------|
| Type                     | Temporary (visual)     | Permanent        |
| Changes original data    | ❌ No                  | ✅ New layer     |
| Used for analysis        | ❌ No                  | ✅ Yes           |
| Output required          | ❌ No                  | ✅ Yes           |

---

## 🧠 Rule of Thumb
- 👁️ Viewing data → On-the-fly is enough  
- 🧪 Running analysis → Use Reproject Layer  
- 💾 Sharing/exporting → Use Reproject Layer  