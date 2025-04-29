# BIPV Facades Dataset

This repository contains a dataset of 400 architectural projects that feature Building-Integrated Photovoltaic (BIPV) Facades. A python notebook is also available for the exploratory data analysis of the curated dataset.  

The goal is to better understand the characteristics, geographical distribution, and temporal evolution of BIPV facades.

---

## Dataset Structure

| Class | Feature Name | Description |
|:------|:-------------------------|:------------|
| **General Information** | country | Country of project location |
|  | region | Region within the country (if available) |
|  | latitude | Latitude (anonymized/generalized) |
|  | longitude | Longitude (anonymized/generalized) |
|  | plant_year | Construction year of the project |
|  | context | Project setting: Urban, Rural, Industrial, Agglomeration, Mountain, Historical |
|  | project_function | Function of the building: Commercial, Educational, Hospital, Industrial, etc. |
|  | project_type | Type of project: New or Retrofit |
| **Technology** | technology | PV technology used: Amorphous Silicon, CIGS, Monocrystalline, Organic PV, Polycrystalline, Thin Film |
|  | installed_power_kWp_ | Installed PV power in kilowatt-peak (kWp) |
|  | surface_area_m2 | Active PV surface area in square meters (m²) |
|  | yield_kWh_per_A | Annual energy yield in MWh per year (MWh/a) |
| **Module Design** | color | Module color: Black, Blue, Bronze, Brown, etc. |
|  | texture | Module surface texture: Flat, Glossy, Metallic, Satin, Structured |
|  | transparency | Transparency level: Opaque, Transparent, Translucent |
|  | module_size | Module size category: Standard, Large, Small, Custom |
|  | module_shape | Module shape: Curved, Mixed, Polygonal, Rectangular, etc. |
|  | cell_visibility | Cell visibility: Visible Cells or Non-Visible Cells |
| **Architectural Integration** | facade_ratio | Ratio of active PV surface to total facade surface (excluding windows) |
|  | inclination_degrees | Inclination of the facade: 0° (horizontal) to 90° (vertical) |
|  | orientation | Orientation: N, NE, E, SE, S, SW, W, NW, or All |
|  | type_of_integration | Type of PV integration: Attached, Rainscreen, Facade Security, Solar Control, Warm Facade |
|  | concept | Design concept: Domination, Imitation, Integration, Subjugation, Subordination |
|  | facade_composition_1 | Primary facade composition: Banner, Depth, Dynamic, Flat, Grid, High Tech, etc. |
|  | facade_composition_2 | Secondary facade composition: Ornament, Sculptural, Skin, ZigZag patterns, etc. |
|  | module_orientation | Module orientation relative to facade: Centric, Horizontal, Vertical, Mixed |
|  | ornamentation | Ornamentation presence: Ornamentation or No Ornamentation |

## Data Anonymization

To respect privacy, confidentiality, and intellectual property considerations:

- Some fields, including **Longitude** and **Latitude**, have been anonymized or generalized to avoid the exact identification of specific projects.
- Contextual information such as **Country**, **Region**, and **Project Attributes** has been retained for analysis purposes but does not allow tracing back to exact building addresses.
- The dataset is intended for research, analysis, and educational purposes only.

By using this dataset, users agree to respect these anonymization measures and use the data in accordance with good scientific and ethical practices.

---

## Exploratory Data Analysis Structure

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
```

## License

This project is licensed under the [MIT License](LICENSE).

## Citation

If you use this dataset or code in your research, please cite it using the Zenodo DOI provided below:

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15301195.svg)](https://doi.org/10.5281/zenodo.15301195)

```bibtex
@misc{duran_bipv_facades_2024,
  author       = {Ayca Duran and Kai Marti and Pedram Mirabian and Christoph Waibel and Arno Schlueter},
  title        = {BIPV Facades Dataset},
  year         = 2025,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.15301195},
  url          = {https://doi.org/10.5281/zenodo.15301195}
}
```
