# Detection of Pipeline Vandalism in Nigeria

## Project Overview

This project uses satellite remote sensing and GIS to detect signs of pipeline vandalism — illegal tapping ("bunkering"), sabotage, and artisanal refining activity — along oil and gas pipeline corridors in the Niger Delta, Nigeria.

## Main Research Question

Where along the pipeline network are vandalism and illegal tapping most likely occurring, based on surface disturbance, thermal anomalies, spill signatures, and proximity to settlements/creeks?

## Key Datasets & Sources

| Dataset | Source |
|---|---|
| Pipeline network routes | NNPC / NOSDRA / OpenStreetMap |
| Oil spill incident records | NOSDRA |
| Optical imagery (change/vegetation stress) | Sentinel-2 |
| SAR imagery (ground disturbance, all-weather) | Sentinel-1 |
| Thermal hotspots (illegal refining fires) | VIIRS / MODIS Active Fire |
| Night-time lights (informal refining clusters) | VIIRS Nighttime Lights |
| Settlement locations | GRID3 Data Hub |
| Rivers/creeks and waterways | OpenStreetMap |
| Land use/land cover | ESA WorldCover |
| Digital Elevation Model (DEM) | OpenTopography / Copernicus GLO-30 |
| Conflict/incident events | ACLED |

## Data Sources & Links

| Dataset | Source | Link |
|---|---|---|
| Oil spill incident records | NOSDRA | https://nosdra.gov.ng/ |
| Pipeline routes (where published) | OpenStreetMap | https://www.openstreetmap.org/ |
| Optical imagery | Copernicus / Sentinel-2 | https://dataspace.copernicus.eu/ |
| SAR imagery | Copernicus / Sentinel-1 | https://dataspace.copernicus.eu/ |
| Active fire / thermal anomalies | NASA FIRMS (VIIRS/MODIS) | https://firms.modaps.eosdis.nasa.gov/ |
| Night-time lights | NOAA VIIRS DNB | https://eogdata.mines.edu/products/vnl/ |
| Settlement locations | GRID3 Data Hub | https://grid3.org/geospatial-data-nigeria |
| Digital Elevation Model (DEM) | OpenTopography / Copernicus GLO-30 | https://portal.opentopography.org/raster?opentopoID=OTSDEM.032021.4326.3 |
| Land use/land cover | ESA WorldCover | https://esa-worldcover.org/en/data-access |
| Conflict/incident events | ACLED | https://acleddata.com/ |

## Methodology (Planned)

1. Digitize or acquire the pipeline network route and buffer it (e.g. 50 m, 100 m, 250 m) to define corridors of interest.
2. Pull historical NOSDRA spill records and geolocate them against the pipeline corridor to establish a baseline of known incidents.
3. Run multi-temporal NDVI/NDWI change detection on Sentinel-2 imagery along the corridor to flag vegetation stress or surface oiling consistent with tapping/spills.
4. Use Sentinel-1 SAR backscatter change detection to catch ground disturbance (excavation, foot traffic, temporary structures) even under cloud cover.
5. Overlay VIIRS/MODIS active-fire and night-time-lights data to flag likely artisanal refining clusters near the corridor.
6. Cross-reference flagged zones with settlement proximity, creek access, and ACLED conflict events to prioritize higher-likelihood vandalism hotspots.
7. Produce a ranked hotspot map of the pipeline corridor for field verification.

## Project Goal

The project aims to combine multi-sensor remote sensing (optical, SAR, thermal, night-lights) with GIS overlay analysis to flag likely pipeline vandalism hotspots for verification and response prioritization.

## Expected Output

The final output will be a GIS-based hotspot map of the pipeline corridor, ranking segments by likelihood of vandalism/illegal tapping activity, cross-referenced with historical NOSDRA spill records.

The project may later be developed into a near-real-time monitoring dashboard.

## Project Status

Week 1 - Project definition and data feasibility completed.
