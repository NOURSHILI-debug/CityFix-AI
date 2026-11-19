# CityFix AI – R3
# Phase 0: Data Sources and License Inventory

## 1. Objective

The objective of this document is to identify and evaluate the data sources required for the CityFix AI project, particularly for the Artificial Intelligence module and geospatial analysis.

The inventory covers three main categories:

- Image datasets for AI-based incident classification.
- Geospatial data for spatial analysis and incident localization.
- Population data for demographic analysis and prioritization.

---

## 2. Image Datasets for AI

### 2.1 RDD2022 – Road Damage Dataset 2022

| Attribute | Description |
|---|---|
| Dataset name | RDD2022 (Road Damage Dataset 2022) |
| Data type | Road damage images |
| Main purpose | Detection and classification of road damage |
| Examples | Potholes, longitudinal cracks, transverse cracks and alligator cracks |
| Official repository | https://github.com/sekilab/RoadDamageDetector |
| Dataset license | Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) |
| Code license | MIT License |

**License conditions:**

The RDD2022 dataset is distributed under the CC BY-SA 4.0 license, which allows free use, modification and commercial use under the following conditions:

- **Attribution (BY):** The original authors must be credited (Deeksha Arya et al. / Sekimoto Lab). The official research publication must also be cited.
- **ShareAlike (SA):** Modified or derived datasets must be redistributed under the same CC BY-SA 4.0 license.

The code and tools available in the official GitHub repository are distributed separately under the MIT License.

**Recommended academic reference:**

Arya, D., Maeda, H., Ghosh, S. K., Toshniwal, D., & Sekimoto, Y. (2022). *RDD2022: A multi-national image dataset for automatic Road Damage Detection.*

- Publication: https://arxiv.org/abs/2209.08538
- Dataset: https://figshare.com/articles/dataset/RDD2022_-_The_multi-national_Road_Damage_Dataset_released_through_CRDDC_2022/21431547

**Role in CityFix AI:**

RDD2022 will be used to develop and evaluate the AI module responsible for identifying road damage, particularly potholes and cracks, from citizen-submitted photographs.

---

### 2.2 TACO – Trash Annotations in Context

| Attribute | Description |
|---|---|
| Dataset name | TACO (Trash Annotations in Context) |
| Data type | Images of waste in real-world environments |
| Main purpose | Waste detection and classification |
| Examples | Plastic bottles, cans, bags and packaging |
| Official repository | https://github.com/pedropro/TACO |
| Annotation license | Creative Commons Attribution 4.0 International (CC BY 4.0) |
| Code license | MIT License |
| Image licenses | Individual licenses depending on the original image source |

**License conditions:**

TACO distinguishes between three types of resources:

- **Annotations:** Bounding boxes and segmentation masks are distributed under CC BY 4.0. They can be reused and modified with appropriate attribution.
- **Individual images:** Images originate from different sources, including Flickr and user contributions. Each image retains its original public license. The source URL and license information are available in the `annotations.json` file. According to the dataset documentation, CC BY 4.0 applies by default when the license field is absent.
- **Code and tools:** The scripts available in the official GitHub repository are distributed under the MIT License.

**Important usage considerations:**

- The original contributors, Pedro F. Proença and Pedro Simões, must be credited when using the dataset.
- The license of each image must be checked individually, especially before redistributing raw images.
- Some images may have additional conditions, such as ShareAlike requirements.

**Official sources:**

- GitHub repository: https://github.com/pedropro/TACO
- Dataset website: http://tacodataset.org/
- Annotations: https://zenodo.org/records/3354286

**Role in CityFix AI:**

TACO will be used to develop and evaluate the AI module responsible for recognizing waste in citizen-submitted photographs, including plastic bottles, cans and other types of litter.

---

## 3. Geospatial Data Sources

### 3.1 OpenStreetMap (OSM)

| Attribute | Description |
|---|---|
| Source | OpenStreetMap |
| Data type | Geospatial vector data |
| Main purpose | Urban spatial analysis and incident localization |
| Available information | Roads, streets, intersections, buildings and points of interest |
| Source website | https://www.openstreetmap.org/ |
| License | Open Database License (ODbL) |

**License conditions:**

OpenStreetMap data is distributed under the Open Database License (ODbL).

The main requirements include:

- Appropriate attribution to OpenStreetMap and its contributors.
- Compliance with ShareAlike requirements when distributing adapted databases.

**Role in CityFix AI:**

OpenStreetMap will provide the geographical information needed to locate incidents, identify nearby roads and infrastructure, and support spatial analysis.

It can also help identify points of interest such as schools and hospitals, depending on data availability.

Administrative boundaries will be obtained from available OpenStreetMap data or additional municipal sources.

---

## 4. Population Data Sources

### 4.1 WorldPop

| Attribute | Description |
|---|---|
| Source | WorldPop |
| Data type | Gridded population data |
| Main purpose | Population distribution and density analysis |
| Available information | Estimated population distribution across geographical areas |
| Source website | https://www.worldpop.org/ |
| License | Creative Commons Attribution 4.0 International (CC BY 4.0) |

**License conditions:**

WorldPop datasets are available under CC BY 4.0, subject to the attribution requirements associated with the selected dataset.

**Role in CityFix AI:**

WorldPop data will help estimate population density in different urban areas.

This information can provide additional context for spatial prioritization and help municipalities understand the potential population affected by reported incidents.

### 4.2 INS – National Institute of Statistics of Tunisia

| Attribute | Description |
|---|---|
| Source | National Institute of Statistics (INS Tunisia) |
| Data type | Official demographic and statistical data |
| Main purpose | Demographic analysis |
| Available information | Population statistics and census information |
| Source website | https://www.ins.tn/ |
| License | Subject to the reuse conditions of the specific dataset |

**Role in CityFix AI:**

INS data will provide official demographic statistics for Tunisia.

It can complement WorldPop data and support population-based analysis at the administrative level.

The specific reuse conditions must be checked for each selected dataset.

---


## 5. Data Usage Considerations

Before integrating the datasets into CityFix AI, the following conditions must be considered:

1. Respect the attribution requirements of each data provider.
2. Verify individual image licenses before redistributing images, particularly for TACO.
3. Respect the ShareAlike requirements associated with RDD2022 and OpenStreetMap.
4. Keep the original source references and license information.
5. Check the specific reuse conditions of INS datasets.
6. Document any modifications made to the original datasets.

---

## 6. Conclusion

The identified data sources provide the foundation for developing the CityFix AI platform.

RDD2022 and TACO will support the development of the AI module for automatically identifying road damage and waste from citizen-submitted photographs.

OpenStreetMap will provide the geographical information required for incident localization and spatial analysis.

WorldPop and INS Tunisia will provide demographic information to support population-based analysis and improve the understanding of urban priorities.

These datasets will be selected and integrated according to their relevance, availability and licensing conditions.


