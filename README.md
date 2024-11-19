# MorphoMap
A custom QGIS tool for morphometric analysis

## In a nutshell

Morphomap is a custom QGIS processing algorithm designed for morphometric analysis. It processes raster layers such as Digital Elevation Models (DEM) and spectral bands to derive slope and Normalized Difference Vegetation Index (NDVI). The results are then exported to a feature sink for further analysis.

## Features

- **Slope Calculation**: Generates a slope layer from the input DEM.
- **NDVI Calculation**: Computes NDVI using the NIR (B08) and Red (B04) bands.
- **Export Results**: Outputs the final NDVI results to a feature sink.

## Getting Started

### Prerequisites

- QGIS with Python support
- Familiarity with QGIS processing framework

### Usage

1. Open QGIS and navigate to the Processing Toolbox.
2. Locate the "Morphomap 2" algorithm under the "Morphometric Analysis" group.
3. Input the required raster layers for DEM, B03, B04, B08, and specify the output feature sink.
4. Run the algorithm and review the outputs.

## Script Overview

The script follows these key steps:

1. **Initialization**: Set up input raster layers (DEM, B03, B04, B08) and the output feature sink.
2. **Slope Calculation**: Generate a slope layer from the DEM raster.
3. **NDVI Calculation**: Calculate NDVI using the formula `(NIR - Red) / (NIR + Red)`, with B08 as the NIR band and B04 as the Red band.
4. **Export Results**: Output the final NDVI results to the specified feature sink.

