# DAS Sepaku Land Cover Mapping (2018)

Technical test submission for This repository contains my technical exercise submission for the Remote Sensing Assistant Technical Test for CIFOR-ICRAF Indonesia. The task focuses on replicating the land cover mapping workflow from the paper:
"A national-scale land cover reference dataset from local crowdsourcing initiatives in Indonesia"
DOI: 10.1038/s41597-022-01689-5

Author: Fannya Rachma Annisa

Repository Contents:
README.md: This file outlining the project overview, implementation steps, encountered challenges, and proposed solutions.

Sepaku_Landcover_2018.js : A costomized Google Earth Engine (GEE) script developed for land cover classification within the Sepaku Watershed, using publicy available reference data.

A. Overall Plan
My strategy to complete this geospatial data processing task was divided into four main stages:

1. Setup and Scoping: Create a new GitHub repository. Carefully analyze the original project structure and the GEE script to understand dependencies, data sources, and the classification workflow.

2. Adaptation for AOI and Time Period: Redefine the Area of Interest (AOI) to focus on the Sepaku sub-watershed in East Kalimantan. Update the script to filter Landsat 8 Surface Reflectance imagery for the year 2018.

3. Blocker Identification and Resolution: Address issues caused by private GEE asset paths. Replace inaccessible assets (e.g., users/hadi/REF_INDO_2019) with equivalent, publicly available CSV data that can be uploaded to Earth Engine (e.g., point samples with lat/lon and land cover labels).

4. Documentation and Finalization: Log all actions, technical decisions, and issues in this README. Clearly distinguish between what was achieved independently and what would require collaboration or domain-specific support.



