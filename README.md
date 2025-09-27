# CMRI-Analysis-ARCGIS-
 The CMRI Map of Sundarban shows the distribution and density of mangroves for 2015, 2020, and 2025.
# 🌳 Combined Mangrove Recognition Index (CMRI) – Sundarban

## 📌 Objective
To accurately distinguish mangrove vegetation from non-mangrove vegetation in the Sundarban region using the Combined Mangrove Recognition Index (CMRI).

## 🗂️ Data Sources
- Landsat 8 OLI/TIRS -137/45,138/45(USGS Earth Explorer)
- Sundarban administrative boundary shapefile
- Software: ArcGIS 10.8 
## 🧮 Formula Used
CMRI is calculated as:
[CMRI = NDVI + MVI]

Where:  
- **NDVI (Normalized Difference Vegetation Index):**  
  \[
  NDVI = {(NIR - RED)}/{(NIR + RED)}
  \]

- **MVI (Mangrove Vegetation Index):**  
  MVI = {(SWIR - GREEN)}/{(SWIR + GREEN)}
  

## 🛠️ Methodology
1. **Preprocessing**  
   - Layer stacking of Landsat bands  
   - Clipping to Sundarban boundary  

2. **Index Calculation**  
   - NDVI from NIR (Band 5) and RED (Band 4)  
   - MVI from SWIR1 (Band 6) and GREEN (Band 3)  
   - CMRI = NDVI + MVI  

3. **Thresholding**  
   - Positive CMRI values = Mangrove vegetation  
   - Negative/low CMRI values = Non-mangrove classes  

4. **Validation**  
   - Cross-check with reference mangrove maps or high-resolution imagery  

## 🗺️ Expected Output
- CMRI raster map showing mangrove vs. non-mangrove areas  
- Statistics of mangrove cover in Sundarban  

<img width="1090" height="713" alt="image" src="https://github.com/user-attachments/assets/0b95a1b5-835e-43c2-a818-e95a34b1d5b4" />

## 📷 Sample Output
<img width="1440" height="768" alt="CMRIiii" src="https://github.com/user-attachments/assets/97c4a31b-7c1e-4e0d-8c75-7e7a6e6cae55" />


