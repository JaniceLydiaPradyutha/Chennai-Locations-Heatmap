# Chennai Traffic Junction Heatmap Analysis Using QGIS

## Overview

This project demonstrates the use of Geographic Information Systems (GIS) to analyze the spatial distribution of major traffic junctions in Chennai. Using QGIS, a heatmap was generated from traffic junction coordinates to visualize traffic density and identify congestion hotspots across the city.

The project uses geographic coordinates along with traffic-related attributes such as traffic volume, congestion level, accident count, and CCTV availability to create an informative spatial visualization that supports urban planning and traffic management.

---

## Objectives

- Visualize the locations of major traffic junctions in Chennai.
- Generate a heatmap to identify high-density traffic areas.
- Analyze traffic congestion patterns using spatial data.
- Demonstrate the application of QGIS for GIS-based traffic analysis.

---

## Software and Tools

- **QGIS 3.x**
- Microsoft Excel
- OpenStreetMap Basemap
- Coordinate Reference System (CRS): **WGS 84 (EPSG:4326)**

---

## Dataset Information

The dataset consists of ten major traffic junctions in Chennai with their geographic coordinates and traffic-related information.

### Dataset Fields

| Field | Description |
|--------|-------------|
| Junction_ID | Unique identifier of the junction |
| Junction_Name | Name of the traffic junction |
| Latitude | Latitude coordinate |
| Longitude | Longitude coordinate |
| Traffic_Volume | Estimated traffic volume |
| Signal_Status | Status of traffic signal |
| Congestion | Congestion level (Medium, High, Very High) |
| Accident_Count | Number of accidents recorded |
| CCTV_Available | CCTV surveillance availability |

### Traffic Junctions Included

- Anna Salai
- T. Nagar Junction
- Guindy Junction
- Velachery Junction
- Tambaram Junction
- Porur Junction
- Koyambedu Junction
- Egmore Junction
- Adyar Junction
- Perambur Junction

---

## Methodology

### 1. Data Preparation

- Created the traffic junction dataset in Microsoft Excel.
- Entered latitude and longitude coordinates for each junction.
- Saved the dataset as a CSV file.

### 2. Import Data into QGIS

- Loaded the CSV file using **Add Delimited Text Layer**.
- Assigned:
  - X Coordinate → Longitude
  - Y Coordinate → Latitude
- Selected **WGS 84 (EPSG:4326)** as the Coordinate Reference System.

### 3. Add Basemap

- Added the OpenStreetMap basemap using the XYZ Tiles option.

### 4. Generate Heatmap

- Opened **Processing Toolbox → Heatmap (Kernel Density Estimation)**.
- Selected the junction point layer as the input.
- Configured the heatmap radius and pixel size.
- Generated the raster heatmap.

### 5. Visualization

- Applied a Blue–Green–Yellow–Red color ramp.
- Displayed junction locations using star symbols.
- Overlaid the heatmap on the OpenStreetMap basemap.

---

## Results

The generated heatmap highlights the concentration of traffic junctions across Chennai.

### High Density Areas

- Anna Salai
- T. Nagar
- Guindy
- Koyambedu
- Perambur

### Moderate Density Areas

- Egmore
- Adyar
- Velachery

### Lower Density Areas

- Tambaram
- Porur

The visualization clearly indicates that Central Chennai contains the highest concentration of major traffic junctions, suggesting increased traffic movement and congestion in these regions.

---

## Applications

- Urban Planning
- Traffic Management
- Smart City Development
- Road Safety Analysis
- Emergency Route Planning
- Infrastructure Planning
- CCTV Surveillance Planning

---
---

## Output

### Input

- CSV dataset containing traffic junction coordinates and traffic attributes.

### Output

- Point layer representing major traffic junctions.
- Heatmap showing traffic density across Chennai.
- Final GIS visualization with OpenStreetMap background.

---

## Future Enhancements

- Integrate real-time traffic data.
- Include road network analysis.
- Perform temporal traffic analysis.
- Analyze accident hotspots using Kernel Density Estimation.
- Publish the map as an interactive web application using QGIS2Web.

---

## Conclusion

This project demonstrates how QGIS can be used to transform geographic coordinate data into meaningful spatial visualizations. The heatmap effectively identifies traffic hotspots across Chennai, providing valuable insights for transportation planning, congestion management, and infrastructure development. The methodology can be extended by incorporating larger datasets and real-time traffic information for more comprehensive urban analysis.

---

## Author

**Project:** Chennai Traffic Junction Heatmap Analysis Using QGIS

**Developed Using:** QGIS 3.x

**Study Area:** Chennai, Tamil Nadu, India

**Author:** Janice Lydia Pradyutha

**Date:** August 2026

---
