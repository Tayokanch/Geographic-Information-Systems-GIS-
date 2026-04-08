# Georeferencing

## Definition
**Georeferencing** is the process of assigning real-world coordinates to a raster image so it can be accurately placed on the Earth’s surface.

---

## Why it’s Important
- Allows images (maps, scans, satellite photos) to align with other GIS data  
- Makes raster data usable for analysis and mapping  
- Ensures spatial accuracy  

---

## Key Idea
A raster image (e.g., scanned map or satellite image) has **no location information by default**.  
Georeferencing “anchors” it to real-world coordinates.

---

## 📍 Use Case Examples
- Adding coordinates to a scanned map so it fits correctly in GIS  
- Positioning a satellite image on the Earth’s surface  
- Aligning an old map with current spatial data  

---

##  How It Works
- Select known locations on the image → called **Ground Control Points (GCPs)** *(also known as tie points)*  
- Match these points to their **real-world coordinates**  
- GIS software uses these points to **transform and align** the image correctly  

---

## 🔑 Key Terms
- **Raster Data** → Pixel-based data (images)  
- **Ground Control Points (GCPs)** → Known reference points with coordinates  
- **Transformation** → Mathematical adjustment to fit the image to real-world space  

---

## ✅ Simple Explanation
👉 Georeferencing = **linking an image to real-world coordinates using known points**

---
