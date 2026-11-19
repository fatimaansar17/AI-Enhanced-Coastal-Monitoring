# AI-Enhanced Coastal Monitoring Using Remote Sensing & GIS

A 34-Year Satellite-Based Shoreline Change Assessment (1990–2024)

*Study Area: Narrabeen–Collaroy Beach, Sydney, Australia*

---

## About the Research

This research investigates long-term shoreline changes along Narrabeen–Collaroy Beach, Sydney, Australia, over a 34-year period (1990–2024). It combines satellite remote sensing, geospatial analysis and artificial intelligence to examine coastal erosion, accretion and shoreline stability.

The study uses multi-temporal satellite imagery and machine learning approaches to support the assessment of coastal dynamics.

## Research Highlights

| Research Component   | Details                             |
| :------------------- | :---------------------------------- |
| Study Period         | 1990–2024                           |
| Satellite Images     | 1,869 candidate scenes              |
| Extracted Shorelines | 1,180                               |
| Study Transects      | 5 (NA1–NA5)                         |
| Study Location       | Narrabeen–Collaroy Beach, Australia |

## Data Sources

- Landsat 5
- Landsat 8
- Landsat 9
- Sentinel-2

## Methodology

**1. Satellite Data Processing**

- Google Earth Engine and Google Colab
- Cloud and shadow masking
- Satellite image preprocessing and quality checks

**2. Shoreline Extraction**

- CoastSat framework
- Modified Normalized Difference Water Index (MNDWI)
- Otsu thresholding
- Sub-pixel shoreline detection

**3. Tidal Correction and Quality Control**

- Fort Denison hourly water-level observations
- Tidal correction using beach slope
- Statistical outlier detection and image-based quality assessment

**4. GIS-Based Shoreline Analysis**

- Net Shoreline Movement (NSM)
- End Point Rate (EPR)
- Linear Regression Rate (LRR)
- Five shore-normal transects

**5. Artificial Intelligence Models**

- Random Forest (100 trees)
- Attention-based U-Net
- Erosion, stable and accretion classification

## Key Research Findings

- Northern shoreline accretion: NA1 (+22.3 m) and NA2 (+18.3 m).
- Consistent erosion at NA5 (−16.5 m).
- Overall beach-wide average net shoreline movement: +3.76 m.

## Model Performance

| Evaluation Metric   | Random Forest | Attention U-Net |
| :------------------ | ------------: | --------------: |
| Test Accuracy       |        89.09% |          92.73% |
| Correct Predictions |         49/55 |           51/55 |

- Random Forest 5-fold cross-validation accuracy: 81.74%.
- Mean positional RMSE against the tidally adjusted shoreline reference: 5.56 m.
- Reference comparison: 597 date-matched observations, with correlation coefficients of 0.888–0.947.

*Note: Model evaluation was conducted at the Narrabeen study site. Cross-site generalisation and temporally blocked validation remain future research directions.*

## Tools & Technologies

`Python` · `Google Earth Engine` · `Google Colab` · `CoastSat` · `QGIS` · `Random Forest` · `Attention U-Net`

## Repository Contents

| File                              | Description                                     |
| :-------------------------------- | :---------------------------------------------- |
| `research_data_preparation.ipynb` | Research data preparation and analysis notebook |

Additional research scripts, model implementations and supporting materials will be organised in this repository as they are prepared for publication.

## Research Objective

To integrate satellite remote sensing, GIS and artificial intelligence for improved understanding and assessment of long-term coastal changes.

---

**Research Area:** Remote Sensing | GIS | Coastal Monitoring | Geospatial AI | Environmental Change Detection
