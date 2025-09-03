# Data Documentation

## 1. Overview
This folder contains the datasets used in the analysis of spatial relationships between health outcomes, environmental amenities, and healthcare accessibility across London neighborhoods.  
Data are organized into two subfolders:  
- `raw/`: Original datasets **not included** due to size restrictions. Users can download them from the official sources listed below.  
- `processed/`: Cleaned, merged, and transformed datasets ready for analysis.  

---

## 2. Data Sources (raw/)
The original raw datasets are sourced from official government and authoritative sources:  

- **Index of Multiple Deprivation (IMD)**  
  - File: `01_IMD.csv`  
  - Source: UK Data Service – [Link](https://data.geods.ac.uk/dataset/index-of-multiple-deprivation-imd/resource/6232c48b-ac82-49ac-a77c-0693a68b33e4)  

- **Points of Interest (POI) Data**  
  - File: `02_poi_uk.gpkg`  
  - Source: Ordnance Survey – [Link](https://docs.os.uk/os-downloads/addressing-and-location/points-of-interest)  

- **London Statistical Boundaries**  
  - Folder: `03_gla`  
  - Source: Greater London Authority – [Link](https://data.london.gov.uk/dataset/statistical-gis-boundary-files-london/)  

- **Greenspace Data**  
  - Folder: `04_OS-Greenspace-data`  
  - Source: OS Open Greenspace Dataset – [Link](https://www.data.gov.uk/dataset/4c1fe120-a920-4f6d-bc41-8fd4586bd662/os-open-greenspace1)  

- **Lower Layer Super Output Areas (LSOA) Boundaries**  
  - Folder: `LSOA_England_2011`  
  - Source: ONS Geography Portal – [Link](https://geoportal.statistics.gov.uk/datasets/ons::lower-layer-super-output-areas-december-2011-boundaries-ew-bfc-v3/about)  

> **Note:** Full raw datasets are not included due to file size limits. Please download them directly from the official sources above.  

---

## 3. Processed Datasets
The `processed/` folder contains the integrated datasets derived from the raw sources. These are directly used in the analysis:  

- `london_health_poi_by_lsoa.csv` – Cleaned and aggregated POI data joined with LSOA boundaries.  
- `london_lsoa_greenspace_analysis.csv.zip` – Green space coverage, proximity, and quality metrics at LSOA level.  
- `london_lsoa_health_scores.csv.zip` – IMD health deprivation scores combined with processed accessibility and environmental measures.  

---

## 4. Data Integration Strategy
Datasets were integrated to form a multi-domain analytical framework capturing:  

- **Health outcomes** through IMD composite indicators.  
- **Environmental factors** via green space coverage and quality indices.  
- **Healthcare accessibility** through geocoded facility locations and classifications.  
- **Spatial context** via standardized administrative boundaries (LSOA and London-specific).  

This integration ensures consistency in data standards, temporal alignment, and spatial accuracy, enabling analysis of complex interactions that single-source datasets cannot capture.  

---

## 5. Notes on Usage
Due to repository size restrictions, full raw datasets are **not included**. Only processed datasets and demonstration files are available. Users requiring full raw data should download them from the official sources listed in Section 2.  

---

## 6. Citation
If you use this dataset, please cite the original data providers (UK Data Service, Ordnance Survey, Greater London Authority, ONS, and data.gov.uk).  
