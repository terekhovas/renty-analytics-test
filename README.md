# Heatmap Generation of Athens Property Data

## Overview
This repository contains Jupyter Notebooks for generating interactive heatmaps of property prices in central Athens, Greece. The data includes properties for sale and rent, with an additional map for Blueground apartments. The heatmaps visualize rental and sales prices, segmented by apartment size and number of bedrooms.

## Features
- **Dynamic Heatmaps**: Visualize rental and sales prices on an interactive map.
- **Layer Control**: Toggle between different apartment categories (e.g., studios, 1-bed, 2-bed apartments).
- **Custom Colormap**: The colormap is adjusted based on the price range of displayed layers.

## Filtering Conditions

### 1. Apartments for Sale
- Price range: €50,000 - €1,000,000
- Area: 20 - 85 sq.m.
- Price per sq.m.: €500 - €10,000

### 2. Long-term Rentals (LTR) Analytics
- Price range: €100 - €5,000
- Area: 20 - 85 sq.m.

## Apartment Segmentation
Apartments are segmented based on size and number of bedrooms:

- **Studio 1-bed apartments**: Less than 30 sq.m.
- **Small 1-bed apartments**: 30 - 45 sq.m.
- **Mid 1-bed apartments**: 45 - 65 sq.m.
- **Large 1-bed apartments**: More than 65 sq.m.
- **Small 2-bed apartments**: 50 - 70 sq.m.
- **Mid 2-bed apartments**: 70 - 85 sq.m.

## Key Functions

### 1. Filtering
The datasets are filtered based on price, area (square meters), and price per square meter. These filters ensure that the analysis focuses on relevant properties in the central Athens area.

### 2. Apartment Segmentation
The `segment_apartments` function segments apartments into different categories based on the number of bedrooms and square footage, such as studios, small 1-bed, mid 2-bed, etc.

### 3. Heatmap Creation
The `create_heatmap_with_layers` function generates interactive heatmaps for each apartment segment, providing a visual representation of property prices in Athens. The heatmaps include:
- Price-based colormap for visualizing rental or sale prices.
- Layer control to toggle between categories.
