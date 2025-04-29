# BIPV Facades Dataset

This repository contains a dataset of 400 architectural projects that feature Building-Integrated Photovoltaic (BIPV) Facades. An exploratory data analysis  of a curated dataset on BIPV facade projects is also available.  
The goal is to better understand the characteristics, geographical distribution, and temporal evolution of BIPV facades.

---

## Dataset Structure

| Class                   | Sub-Class       | Attributes |
|:-------------------------|:----------------|:-----------|
| **General Information**  | Location         | Country, Region, Longitude, Latitude |
|                          | Year              | Construction Year |
|                          | Context           | Urban, Rural, Industrial, Agglomeration, Mountain, Historical |
|                          | Project Function  | Commercial, Educational, Hospital, Industrial, Institutional, Multifunctional, Office, Public, Residential, Sport |
|                          | Project Type      | New, Retrofit |
| **Technology**           | Technology        | Amorphous Silicon, CIGS, Monocrystalline, Organic PV, Polycrystalline, Thin Film |
|                          | Installed Power   | Installed power in kWp |
|                          | Surface           | PV surface area in m² |
|                          | Annual Yield      | Energy yield in MWh/a |
| **Module Design**        | Color             | Black, Blue, Bronze, Brown, Gold, Green, Grey, Multi, Orange, Print, Purple, Red, White |
|                          | Texture           | Flat, Glossy, Metallic, Satin, Structured |
|                          | Transparency      | Opaque, Transparent, Translucent |
|                          | Module Size       | Standard, Large, Small, Custom |
|                          | Module Shape      | Curved, Mixed, Polygonal, Rectangular, Rhomboid, Square, Triangular |
|                          | Cell Visibility   | Visible Cells, Non-Visible Cells |
| **Architectural Integration** | Facade Ratio  | Active PV Surface / Total Facade Surface (excluding windows) |
|                          | Inclination       | 90° (Vertical) to 0° (Horizontal) |
|                          | Orientation       | N, NE, E, SE, S, SW, W, NW, All |
|                          | Type of Integration | Attached, Facade Security, Rainscreen, Solar Control, Warm Facade |
|                          | Design Concept    | Domination, Imitation, Integration, Subjugation, Subordination |
|                          | Facade Composition| Banner, Depth, Dynamic, Flat, Grid, High Tech, Media, Ornament, Rhythmic, Sculptural, Skin, Vertical ZigZag, Horizontal ZigZag |
|                          | Module Orientation| Centric, Horizontal, Mixed, Vertical |
|                          | Ornamentation     | Ornamentation, No Ornamentation |

---

## Structure

- **Preprocessing:**  
  - Data cleaning
  - Missing value visualization 
- **Numerical Feature Analysis:**  
  - Histograms, boxplots, and violin plots for numerical attributes
- **Categorical Feature Analysis:**  
  - Histograms for categorical attributes
- **Spatial Analysis:**  
  - Map showing project counts across countries
- **Temporal Trends:**  
  - Labeled heatmaps showing how facade features evolved over time

---

## Installation

1. Clone this repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
