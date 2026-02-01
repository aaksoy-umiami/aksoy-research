---
layout: single
title: "" # Leave empty so we can use the custom excerpt below
permalink: /tools/hurricane-data/
layout: single
author_profile: true
toc: true
toc_label: "Page Contents"
excerpt: >
  <span style="display: block; font-size: 2.0em; font-weight: bold; color: white; line-height: 1.2;">Tools > Hurricane Observations Datasets</span>
header:
  overlay_color: "#000"
  overlay_filter: 0.1
  overlay_image: https://raw.githubusercontent.com/mmistakes/minimal-mistakes/master/assets/images/header-bg.jpg
---

<div class="notice--info">
  <strong>Status: Active Development</strong><br>
  This project is currently in the active data engineering phase. We are working to release the first version of the standardized dataset in late 2026.
</div>

## The Mission: "AI-Ready" Hurricane Data
For decades, NOAA’s Hurricane Research Division (HRD) and the National Hurricane Center (NHC) have collected invaluable inner-core observations from aircraft reconnaissance. However, this data exists in disparate formats, legacy archives, and varying standards that make it difficult to use in modern machine learning (ML) and data assimilation applications.

**This project aims to unify these disparate sources into a single, standardized, and "AI-Ready" dataset.**

By converting decades of raw flight-level and dropwindsonde data into modern, self-describing formats (NetCDF/HDF5), we are building the foundational infrastructure required to train the next generation of deep learning models for tropical meteorology.

## The Challenge
* **Disparate Sources:** Data is scattered across multiple agencies (NOAA, USAF Reserves) and archival systems.
* **Legacy Formats:** Much of the historical data exists in ASCII text files or proprietary binary formats that require specialized decoding.
* **Inconsistent Metadata:** Variable names, units, and quality control flags have changed repeatedly over the last 30 years.

## Methodology & Goals
We are building a robust processing pipeline to standardize this data:

1.  **Ingestion:** Aggregating high-density observations (HDOBS), dropwindsondes, and tail-Doppler radar data.
2.  **Standardization:** Mapping all physical quantities to a unified schema with consistent units and CF-compliant metadata.
3.  **Quality Control:** Implementing automated QC flags to identify instrument errors and outliers.
4.  **Distribution:** Outputting the final product in cloud-optimized NetCDF/HDF5 formats accessible via Python/Xarray.

## Future Access
* **Code Repository:** Scripts for decoding and standardizing raw flight data will be released on GitHub.
* **Data Access:** The curated dataset will be hosted on NOAA/NCEI repositories with public access.

*For inquiries regarding collaboration or early access to data samples, please [contact me](/contact/).*

---
**[← Back to Tools & Software](/tools/)** |  [Go to Home](/)
