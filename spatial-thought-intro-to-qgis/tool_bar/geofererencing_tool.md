# 🗺️ Georeferencing Transformations in QGIS 

## 📌 Overview
When georeferencing in QGIS, **transformation types** define how your image is mathematically adjusted to fit real-world coordinates.

Each method varies in:
- Accuracy
- Flexibility
- Number of points required

---

## 🔧 Common Transformation Types

### 1. 🟢 Linear (Helmert)
**What it does:**
- Applies simple shift, rotation, and scaling

**Best used when:**
- Image is already fairly accurate  
- Only small adjustments are needed  

**GCPs required:** Minimum 2  

---

### 2. 🔵 Polynomial 1 (Affine)
**What it does:**
- Allows scaling, rotation, shifting, and skewing

**Best used when:**
- Most common choice  
- Image has slight distortion  

**GCPs required:** Minimum 3  

👉 **Default & recommended for beginners**

---

### 3. 🟡 Polynomial 2
**What it does:**
- Handles moderate warping (curved distortion)

**Best used when:**
- Old maps or slightly distorted images  
- When affine isn’t accurate enough  

**GCPs required:** Minimum 6  

---

### 4. 🟠 Polynomial 3
**What it does:**
- Handles complex distortion (more flexible warping)

**Best used when:**
- Highly distorted maps  
- Historical or scanned documents  

**GCPs required:** Minimum 10  

⚠️ Can overfit if too many points are inaccurate

---

### 5. 🔴 Thin Plate Spline (TPS)
**What it does:**
- Warps image to pass exactly through all GCPs

**Best used when:**
- Image has irregular/local distortions  
- Maximum visual accuracy is needed  

**GCPs required:** Many  

⚠️ Very sensitive to bad points (can distort heavily)

---

### 6. 🟣 Projective
**What it does:**
- Corrects perspective distortion (like tilted photos)

**Best used when:**
- Aerial images taken at an angle  
- Photos with perspective issues  

**GCPs required:** Minimum 4  

---

## 📊 Quick Comparison

| Transformation      | Use Case                     | GCPs | Complexity |
|--------------------|----------------------------|------|-----------|
| Linear (Helmert)   | Minor adjustments           | 2    | Low       |
| Polynomial 1       | General use (recommended)   | 3    | Low       |
| Polynomial 2       | Moderate distortion         | 6    | Medium    |
| Polynomial 3       | High distortion             | 10   | High      |
| Thin Plate Spline  | Local warping               | Many | Very High |
| Projective         | Perspective correction      | 4    | Medium    |

---

## 🎯 Best Practice
- Start with **Polynomial 1 (Affine)**  
- Only move to higher-order transformations if needed  
- Ensure GCPs are:
  - Well distributed  
  - Accurate  
  - Not clustered  

---

## ✅ Key Takeaway
👉 Choose the **simplest transformation that gives acceptable accuracy**—more complex doesn’t always mean better.