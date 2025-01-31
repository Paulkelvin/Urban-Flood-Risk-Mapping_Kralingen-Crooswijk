
# 🌍 Flood Risk Assessment: Kralingen-Crooswijk, Rotterdam  
*A GIS-based flood vulnerability analysis for urban resilience planning.*  
**Project Link:** [Urban Flood Risk Mapping Of Kralingen-Crooswijk](https://paulkelvin.github.io/Urban-Flood-Risk-Mapping_Kralingen-Crooswijk/)

## Table of Contents

* [Project Overview](#project-overview)
* [Data & Methodology](#data--methodology)
    * [Data Sources](#data-sources)
    * [Methodology](#methodology)
* [Key Outputs](#key-outputs)
* [Results](#results)
    * [Map Imagery Of Affected Assets](#Map-Imagery-Of-Affected-Assets)
    * [Land Use Summary](#land-use-summary)
        * [Land Use Summary of the Study Area](#land-use-summary-of-the-study-area)
        * [Land Use Summary of Flood Extent](#land-use-summary-of-flood-extent)
    * [Key Observations](#key-observations)
* [References](#references) 
* [Contributing](#contributing)
* [License](#license)

---

## Project Overview  
This project identifies **critical flood-prone zones** in Kralingen-Crooswijk, Rotterdam, using a weighted overlay model. The analysis integrates:  
- **Land Elevation** (25% weight)  
- **Flow Accumulation** (30% weight)  
- **Slope** (15% weight)  
- **Proximity to Water Bodies** (20% weight)  
- **Land Use** (10% weight)  

**Formula**:  

Flood Risk Index = (0.30 * Flow Accumulation) + (0.15 * Slope)  
                + (0.25 * Elevation) + (0.20 * Water Body Proximity)  
                + (0.10 * Land Use)  
## Data & Methodology

### Data Sources

| Dataset              | Source              |
|----------------------|----------------------|
| Elevation (AHN4)     | PDOK Netherlands    |
| Land Use            | Overpass Turbo    |
| Roads & Buildings    | OpenStreetMap (OSM) |
| watershed Boundary    |       KNMI         |

## Methodology

### Data Preprocessing:

* Reclassified raster layers into 3 risk classes (1=high, 2=medium, 3=low).
* All classes in output(Flood extent) classified as Flood prone

### Weighted Overlay:

* Combined layers in QGIS using the formula above.

### Validation:

* Cross-referenced with historical flood data from Dutch Water Authorities.

## Key Outputs

1.  **Flood Risk Zonation**
2.      * Flood extent

3.  **Asset Exposure**
       ### Exposed Assets
      
      * **Residential:**
          * Houses: 69
          * Apartments: 61
          * Houseboats: 22 
      * **Commercial:** 4
      * **Industrial:** 15
      * **Schools:** 2
      * **Service:** 6
      * **Sheds:** 2
      * **Water Tower:** 1

**Key Observations:**
* Residential buildings are the most affected category, with houses and apartments accounting for a significant portion of the total.
* The presence of houseboats among the affected buildings highlights the vulnerability of this specific type of residential structure in flood-prone areas.
* Commercial and industrial buildings are also affected, indicating potential economic impacts of flooding.
* Critical infrastructure like schools is also at risk, emphasizing the need for flood mitigation and preparedness measures.

## 📊 Results

### Map Imagery Of Affected Assets
## Distribution of Critical Infrastructure Affected By Flood in Kralingen-Crooswijk
### Map images can be found in Asset folder
## Map of Flood Extent in Kralingen-Crooswijk
![Map of Flood Extent](https://raw.githubusercontent.com/Paulkelvin/Urban-Flood-Risk-Mapping_Kralingen-Crooswijk/master/Asset/Map-of-Flood-Extent-in-Kralingen-Crooswijk_11zon.png)

## Map Of Road Network In Kralingen-Crooswijk
![Map Of Road Network](https://raw.githubusercontent.com/Paulkelvin/Urban-Flood-Risk-Mapping_Kralingen-Crooswijk/master/Asset/Map-Of-Road-Network-In-Kralingen-Crooswijk_11zon.png)

## Map Of Road Network (Safe Roads)
![Safe Roads](https://raw.githubusercontent.com/Paulkelvin/Urban-Flood-Risk-Mapping_Kralingen-Crooswijk/master/Asset/Map-Of-Road-Network-In-Kralingen-Crooswijk-safe-roads_11zon.png)

## Distribution of Critical Infrastructure
![Critical Infrastructure](https://raw.githubusercontent.com/Paulkelvin/Urban-Flood-Risk-Mapping_Kralingen-Crooswijk/master/Asset/Distribution-of-Critical-Infrastructure-in-Kralingen-Crooswijk_11zon.png)

## Critical Infrastructure Affected by Flood
![Critical Infrastructure Flood](https://raw.githubusercontent.com/Paulkelvin/Urban-Flood-Risk-Mapping_Kralingen-Crooswijk/master/Asset/Distribution-of-Critical-Infrastructure-Affected-By-Flood-in-Kralingen-Crooswijk_11zon.png)

## Land Use Types Affected by Flood
![Land Use Types](https://raw.githubusercontent.com/Paulkelvin/Urban-Flood-Risk-Mapping_Kralingen-Crooswijk/master/Asset/Distribution-of-Land-Use-Types-Affected-By-Flood-In-Kralingen-Crooswijk_11zon.png)

# Land Use Summary
## Land Use Summary of the Study Area

| Land Use   | Area (sq. meters) | Percentage of Total Area |
|------------|------------------|-------------------------|
| Residential | 5,026,782.75     | 81.2%                  | 
| Commercial  | 357,973.44      | 5.8%                  |
| Industrial  | 583,974.69      | 9.4%                  |
| Farmland   | 3,401.73        | 0.1%                  |
| Allotments  | 186,868.85      | 3.0%                  | 
| **Total**    | 6,159,001.47     | 100.0%                 |


## Land Use Summary of Flood Extent

| Land Use   | Area (sq. meters) | Percentage of Total Area |
|------------|------------------|-------------------------|
| Residential | 725,063.35     | 80.6%                  | 
| Commercial  | 342,125.86      | 5.5%                  |
| Industrial  | 171,979.10      | 2.8%                  |
| Farmland   | 1,138.90        | 0.0%                  |
| **Total**    | 1,240,307.20     | 100.0%                 |


### Key Observations 

* **Residential areas are disproportionately affected by flooding.** While residential land use accounts for 81.2% of the total study area, it comprises 80.6% of the area directly impacted by the flood. This highlights the vulnerability of residential zones to flood events.
* **Commercial and Industrial areas are also impacted, but to a lesser extent than their overall coverage.** This suggests that these areas might be located in less flood-prone zones within the study area.
* **Farmland and allotments have a relatively minor proportion within both the total area and the flooded extent.** This indicates that these land uses are relatively less vulnerable to flooding in this particular context.
* **The overall land use distribution in the study area is dominated by residential areas, followed by industrial and commercial zones.** This context is important for understanding the potential impact of flooding on different sectors and communities.

### References
### Contributing
### License
