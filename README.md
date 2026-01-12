# Earthquake Data Engineering Project with Microsoft Fabric

## Overview
This project demonstrates an **end-to-end data engineering and analytics pipeline** built on **Microsoft Fabric**, leveraging its **Data Factory, Data Engineering, and Power BI** workloads.

Real-time **earthquake event data** is ingested from the **USGS Earthquake API**, processed through medallion architecture (**Bronze → Silver → Gold**), and visualized for analytical insights.

**Key Capabilities:**
- API ingestion with Fabric Notebooks
- PySpark-based data processing
- Medallion architecture implementation
- Visualization and BI reporting

---

## Technologies Used
- **Microsoft Fabric**
  - Data Factory (Pipelines, Dataflows Gen2)
  - Data Engineering (Notebooks, Spark)
  - Power BI (Gold layer reporting)
- **Python**
- **PySpark**

---

## Repository Structure

### 1. Bronze Layer – Raw Ingestion
`Worldwide Earthquake Events API - Bronze Layer Processing`

- Ingests raw JSON from USGS API
- Minimal processing
- Stores data in original structure for traceability

### 2. Silver Layer – Cleansing & Transformation
`Worldwide Earthquake Events API - Silver Layer Processing`

- Cleans and normalizes raw data
- Handles schema alignment
- Produces refined analytical datasets

### 3. Gold Layer – Analytics & Modeling
`Worldwide Earthquake Events API - Gold Layer Processing`

- Business-ready datasets
- Optimized for Power BI models
- Supports reporting and geospatial analysis

---

## Data Attributes

| Field | Type | Description |
|---|---|---|
| `id` | string | Unique record identifier |
| `latitude` | double | Event latitude |
| `longitude` | double | Event longitude |
| `elevation` | double | Elevation in meters |
| `title` | string | Event title or summary |
| `place_description` | string | Descriptive location |
| `sig` | bigint | Significance score |
| `mag` | double | Earthquake magnitude |
| `magType` | string | Magnitude type (e.g., MB, MW) |
| `time` | timestamp | Event timestamp |
| `updated` | timestamp | Last update timestamp |

---

## Getting Started

To explore or reproduce the project:

1. Clone this repository
2. Open notebooks in **Microsoft Fabric Data Engineering**
3. Configure the USGS API endpoint (if needed)
4. Execute notebooks in sequence:
   - Bronze → Silver → Gold
5. Build reports using **Power BI in Fabric**

---

## Prerequisites
- Microsoft Fabric account
- (Optional) Fabric Admin or workspace admin access
- Basic knowledge of:
  - Python / Spark
  - Data engineering concepts
  - Power BI visualization

---

## Data Source
Earthquake events data provided by:
- **USGS Earthquake Hazards Program**

---

![Image](https://github.com/user-attachments/assets/fb52aa09-7a28-47fa-866d-1eec2e6fd91a)
![Image](https://github.com/user-attachments/assets/9993dd57-e210-4222-9a4e-7648ce446ddc)
![Image](https://github.com/user-attachments/assets/fb581600-5f7c-4aeb-8aa8-1574cc4576d1)
