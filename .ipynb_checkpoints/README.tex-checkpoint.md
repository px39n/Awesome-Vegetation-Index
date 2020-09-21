# Awesome Vegetation Index [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
List of dissertations, application, software related to Vegetation Indices.
<img src="https://flurosat.com/wp-content/uploads/2018/10/growth-monitoring-e1583902228867.png)" alt="drawing" width="600"/>

## Table of Contents

<!-- Start TOC (do not remove me) -->
- [Literature Reviews](#literature-reviews)
- [Vegetation Index for Broadband](#vegetation-index)
  - [Broadband Greenness and Cover](#roadband-greenness-and-cover)
  - [UAV Greenness](#uav-greenness)
  - [Light Use Efficiency](#llight-use-efficiency)
  - [Canopy Nitrogen](#canopy-nitrogen)
  - [Dry or Senescent Carbon](#dry-or-senescent-carbon)
  - [Leaf Pigments](#leaf-pigments)
  - [Canopy Water Content](#canopy-water-content)
- [Hyperspectral Vegetation Index](#hyperspectral-egetation-Index)
- [Community](#community)
  - [Learning Materials](#learning-materials)
- [Software](#Software)
  - [Commercial](#Commercials)
  - [Open](#Open)
 
<!-- End TOC (do not remove me) -->

<!-- Start Links (do not remove me) -->
## Literature Reviews
1. Significant Remote Sensing Vegetation Indices: A Review of Developments and Applications ([li et al. 2017](https://www.hindawi.com/journals/js/2017/1353691/))
2. Research on Vegetation Information Extraction from Visible UAV Remote Sensing Images ([yuan et al. 2018](https://ieeexplore.ieee.org/document/8598637))
3. Hyperspectral vegetation indices and their relationships with agricultural crop characteristics([Thenkabail et al.2000](http://apps.webofknowledge.com/full_record.do?product=UA&search_mode=GeneralSearch&qid=8&SID=5AYEOj1lDfu8CskvSSI&page=2&doc=17))
4. Evaluating Multispectral Images and Vegetation Indices for Precision Farming Applications from UAV Images ([Candiago et al. 2015](https://www.mdpi.com/2072-4292/7/4/4026))

## Vegetation Index

### Broadband  Greenness and Cover
Broadband greenness measures the health of vegetation leaf area index (LAI) and canopy chlorophyll density (CCD) vegetation cover, LAI, biomass, growth, and vigor assessment. It is worthy noting that the selection of proper wavebands in hyperspectral data could partly compensate the limitations of some VI formulas.[(Zhao et al.2007)](https://www.sciencedirect.com/science/article/abs/pii/S0924271607000056)

*Table1. Common Greenness Indices for Broadband*

Name| Abbrev. | Formula | Atmospheric Effects Parameters | Soil Adjustment Parameters| Reference
---|---|---|---|---|---
Normalized Difference Vegetation Index | NDVI |$\frac{R_{\mathrm{NIR}}-R_{\mathrm{Red}}}{R_{\mathrm{NIR}}+R_{\mathrm{Red}}}$|Pigment, Canopy | | [paper](https://scholar.google.com/scholar_lookup?title=Monitoring%20vegetation%20systems%20in%20the%20great%20plains%20with%20erts&author=J.%20W.%20Rouse%20Jr.&author=R.%20Haas&author=J.%20Schell&author=&author=D.%20Deering&publication_year=1974))
The Wide Dynamic Range Vegetation Index|WDRVI | $\frac{a \times R_{N I R}-R_{N I R}}{a \times R_{\mathrm{NIR}}+R_{\mathrm{Red}}}$
Simple Ratio  | SR| $\frac{\text { Near Infrared }}{\text { Red }}$ 
Atmospherically Resistant Vegetation Index | ARVI|$\frac{R_{\mathrm{NIR}}-\left(R_{\mathrm{Red}}-\gamma\left(R_{\mathrm{B} \mathrm{lue}}-R_{\mathrm{Hed}}\right)\right)}{R_{\mathrm{NIR}}+\left(R_{\mathrm{Red}}-\gamma\left(R_{\mathrm{Blue}}-R_{\mathrm{Red}}\right)\right)}$ | γ| | 
soil and atmosphere resistant vegetation|SARVI|$\frac{R_{\mathrm{NIR}}-\left(R_{\mathrm{Red}}-\gamma\left(R_{\mathrm{Blue}}-R_{\mathrm{Red}}\right)\right)}{R_{\mathrm{NIR}}+\left(R_{\mathrm{Red}}-\gamma\left(R_{\mathrm{Blue}}-R_{\mathrm{Red}}\right)\right)+L}(1+L)$ | γ|L | 
modified soil and atmosphere resistant vegetation|MSARVI| $\frac{R_{\mathrm{NIR}}-R_{\mathrm{Red}}}{R_{\mathrm{NIR}}+R_{\mathrm{Red}}+L^{\prime}}\left(1+L^{\prime}\right)$| γ| | 
atmosphere effect resistant vegetation|IAVI|$\frac{R_{\mathrm{NIR}}-\left[R_{\mathrm{Red}}-\gamma^{\downarrow}\left(R_{\mathrm{Blue}}-R_{\mathrm{Red}}\right)\right]}{R_{\mathrm{NIR}}+\left[R_{\mathrm{Red}}-\gamma^{\downarrow}\left(R_{\mathrm{Blue}}-R_{\mathrm{Red}}\right)\right]}$ | γ|L |  
Enhanced Vegetation Index | EVI| $\frac{R_{\mathrm{NIR}}-R_{\mathrm{Red}}}{R_{\mathrm{NIR}}+C_{1} R_{\mathrm{Red}}-C_{2} R_{\mathrm{Blue}}+L}(1+L)$| C1|L |  
Perpendicular Vegetation Index| PVI|$\frac{1}{\sqrt{M^{2}+1}}\left(R_{\mathrm{NIR}}-M \times R_{\mathrm{Red}}-I\right)$ | |M,I | 
Soil Adjusted Vegetation Index| SAVI|$\frac{R_{\mathrm{NIR}}-R_{\mathrm{Red}}}{R_{\mathrm{NIR}}+R_{\mathrm{Red}}+L}(1+L)$ | |L| 
Transformed Soil Adjusted Vegetation Index| TSAVI|$\frac{M\left(R_{\mathrm{NIR}}-M\right)\left(R_{\mathrm{Red}}-L\right)}{R_{\mathrm{Red}}+M \times R_{\mathrm{NIR}}-M \times L}$ | |M,L| 
Modified Soil Adjusted Vegetation Index| MSAVI|$\frac{R_{\mathrm{NIR}}-R_{\mathrm{Red}}}{R_{\mathrm{NIR}}+R_{\mathrm{Red}}+L^{\prime}}\left(1+L^{\prime}\right)$ | |L'| 
Optimized Soil Adjusted Vegetation Index| OSAVI|$\frac{R_{\mathrm{NIR}}-R_{\mathrm{Red}}}{R_{\mathrm{NIR}}+R_{\mathrm{Red}}+\theta}$ | |θ| 
generalized soil-adjusted vegetation index| GESAVI|$\frac{R_{\mathrm{NIR}}-M \times R_{\mathrm{Red}}-L}{R_{\mathrm{Red}}+Z}$ | |L,M,Z| 
Global Environmental Monitoring _Index_| GEMI|$\eta(1-0.25 \eta)-\frac{R_{\mathrm{Red}}-0.125}{1-R_{\mathrm{Red}}}$ | |n| 
Chlorophyll Absorption Ratio Index | CARI | $\left(\frac{700 \mathrm{nm}}{670 \mathrm{nm}}\right) \frac{\sqrt{(a \cdot 670+670 \mathrm{nm}+b})}{\left(a^{2}+1\right)^{0.5}}$
Modified Chlorophyll Absorption Ratio Index | MCARI | 
Difference Vegetation Index|DVI | $R_{\mathrm{NIR}}-R_{\mathrm{Red}}$
weighted Difference Vegetation Index|WDVI|$R_{\mathrm{NIR}}-M \times R_{\mathrm{Red}}$| |L |  
Renormalized Difference Vegetation Index|RDVI|$\sqrt{N D V I \times D V I}$

*Parameter:
M: Slope of soil baseline 
I: Intercept of soil baseline 
L: Soil conditioning index
L': A formula need to be added
θ: SAIL constant 0.16
n: Atmospheric Regulation Factor(C =6、C =7．5)
y: Atmospheric radiation correction coefficient*

### UAV Greenness
Name| Abbrev. | Formula | Atmospheric Effects Parameters | Soil Adjustment Parameters| Reference
---|---|---|---|---|---
Normalized Difference Vegetation Index | NDVI |$\frac{R_{\mathrm{NIR}}-R_{\mathrm{Red}}}{R_{\mathrm{NIR}}+R_{\mathrm{Red}}}$|Pigment, Canopy | | [paper](https://scholar.google.com/scholar_lookup?title=Monitoring%20vegetation%20systems%20in%20the%20great%20plains%20with%20erts&author=J.%20W.%20Rouse%20Jr.&author=R.%20Haas&author=J.%20Schell&author=&author=D.%20Deering&publication_year=1974))
Visible-band difference vegetation index |VDVI| $\frac{\left(2 * \rho_{\text {green }}-\rho_{\text {red }}-\rho_{\text {blue }}\right)}{\left(2 * \rho_{\text {green }}+\rho_{\text {red }}+\rho_{\text {blue }}\right)}$
Normalized green-blue difference index | NGBDI |
Normalized green-red difference index | NGRDI
Red-green ratio index |RGRI
Blue Green ratio index| BGRI
Excess green|EXG
Excess red | EXR
excess green minus excess red|EXGR
color index of vegetation extraction|CIVE
Red green blue vegetation index | RGBVI


### Light Use Efficiency (Disease detection)
Name| Abbrev. | Formula | Atmospheric Effects Parameters | Soil Adjustment Parameters| Reference
---|---|---|---|---|---
Photochemical Reflectance Index|PRI
Structure Insensitive Pigment Index|SIPI

###  Canopy Nitrogen
Name| Abbrev. | Formula | Atmospheric Effects Parameters | Soil Adjustment Parameters| Reference
---|---|---|---|---|---
Normalized Difference Nitrogen Index | NDNI

###  Dry or Senescent Carbon
Name| Abbrev. | Formula | Atmospheric Effects Parameters | Soil Adjustment Parameters| Reference
---|---|---|---|---|---
Normalized Difference Lignin Index|NDLI
Plant Senescence Reflectance Index|PSRI

###  Leaf Pigments
Name| Abbrev. | Formula | Atmospheric Effects Parameters | Soil Adjustment Parameters| Reference
---|---|---|---|---|---
Carotenoid Reflectance Index 1|CRI1
Anthocyanin Reflectance Index 1|ARI1
Anthocyanin Reflectance Index 2|ARI2


###  Canopy Water Content
Name| Abbrev. | Formula | Atmospheric Effects Parameters | Soil Adjustment Parameters| Reference
---|---|---|---|---|---
Water Band Index|WBI
Normalized Difference Water Index|NDWI
Moisture Stress Index|MSI
Normalized Difference Infrared Index|NDII



## Hyperspectral Vegetation Index
The overall amount and quality of photosynthetic material in vegetation.

| NAME                                                    | INDEX(series)       | FORMULA (sample)                                                                                         | SENSITIVITY           | Reference                          |
|---------------------------------------------------------|---------------------|----------------------------------------------------------------------------------------------------------|-----------------------|------------------------------------|
| Improved SAVI with self-adjustment factor L             | MSAVI               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$  | Canopy structure      | Qi et al. (1994)                   |
| Modified Triangular Vegetation Index                    | MTVI1,MTVI2         | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Haboudane et al. (2004)            |
| Normalized Difference Vegetation Index                  | gNDVI,hNDVI, etc    | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Rouse et al. (1974)                |
| Optimized Soil Adjusted Vegetation Index                | OSAVI               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Rondeaux et al. (1996)             |
| Renormalized Difference Vegetation Index                | RDVI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Rougean and Breon (1995)           |
| Simple Ratio Index                                      | SR,SR705            | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Jordan (1969); Rouse et al. (1979) |
| Soil Adjusted Vegetation Index                          | SAVI,SAVI2          | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Huete (1988)                       |
| Spectral Polygon Vegetation Index                       | SPVI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Vincini et al. (2006)              |
| Thematic Mapper NDVI                                    | tmNDVI              | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Rouse et al. (1974)                |
| Transformed Soil Adjusted Vegetation Index              | TSAVI               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Canopy structure      | Baret et al. (1989)                |
| Anthocyanin Reflectance Index                           | ARI                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Carotenoid content    | Gitelson et al. (2002)             |
| Pigment Specific Simple Ratio for Carotenoids           | PSSRc               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Carotenoid content    | Blackburn (1998)                   |
| Structural Independent Pigment Index                    | SIPI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Carotenoid content    | Penuelas and Filella (1998)        |
| Carter Stress Index                                     | CSI1,CSI2           | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Carter (1994)                      |
| Chlorophyll Absorption Integral                         | CAI,CRI,CRI2        | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Oppelt and Mauser (2003)           |
| Gitelson & Merzlyak Index                               | GM1,GM2             | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Gitelson and Merzlyak (1997)       |
| Leaf Chlorophyll Index                                  | LCI,LIC1,LIC2,LIC3  | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Datt (1999)                        |
| M Locherer Chlorophyll                                  | MLO                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | unpublished                        |
| Modified Chlorophyll Absorption in Reflectance Index    | MCARI,MCARI1,MCARI2 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Daughtry et al. (2000)             |
| Normalized Phaeophytinization Index                     | NPQI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Barnes (1992)                      |
| Photochemical Reflectance Index                         | PRI                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Gamon et al. (1992)                |
| Red Edge Inflection Point                               | REIP1               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Guyot et al. (1988)                |
| Red Edge Point                                          | REP                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Dawson and Curran (1998)           |
| Transformed Chlorophyll Absorption in Reflectance Index | TCARI               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Haboudane et al. (2002)            |
| Triangular Vegetation Index                             | TVI                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Broge and Leblanc (2000)           |
| Vogelmann Index                                         | VOG1,VOG2,VOG3      | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Vogelmann (1993)                   |
| Zarco-Tejada & Miller                                   | ZTM                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll           | Zarco-Tejada et al. (2001)         |
| Pigment Specific Simple Ratio for Chl a                 | PSSRa               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll a         | Blackburn (1998)                   |
| Pigment Specific Simple Ratio for Chl b                 | PSSRb               | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Chlorophyll b         | Blackburn (1998)                   |
| Shortwave Infrared Green Vegetation Index               | SWIRVI              | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Dry Matter            | Lobell et al. (2001)               |
| Normalized Difference Lignin Index                      | NDLI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Dry Matter / Lignin   | Serrano et al. (2002)              |
| Normalized Difference Nitrogen Index                    | NDNI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Dry Matter / Nitrogen | Serrano et al. (2002)              |
| Normalized Pigment Chlorophyll Index                    | NPCI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Dry Matter / Pigment  | Penuelas et al. (1994)             |
| Pigment Index                                           | BGI,BRI             | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Dry Matter / Pigment  | Zarco-Tejada et al. (2005)         |
| Red-Green Pigment Index                                 | RGI                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Dry Matter / Pigment  | Zarco-Tejada et al. (2005)         |
| Simple Ratio Pigment Index                              | SRPI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Dry Matter / Pigment  | Penuelas et al. (1995)             |
| Desease Water Stress Index                              | DSWI,DWSI5          | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Water Content         | Galvão et al. (2005)               |
| Leaf Water Vegetation Index                             | LWVI1,LWVI2         | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Water Content         | Galvão et al. (2005)               |
| Moisture Stress Index                                   | MSI                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Water Content         | Hunt et al. (1989)                 |
| Normalized Difference Water Index                       | NDWI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Water Content         | Gao (1996)                         |
| Plant Water Index                                       | PWI                 | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Water Content         | Penuelas et al. (1997)             |
| Simple Ratio Water Index                                | SRWI                | $\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Water Content         | Zarco-Tejada et al. (2003)         |
                                                         |                     | 

## Community

### Learning Materials

* [Index Database](https://www.indexdatabase.de/) - An Index-Data-Base (IDB) could be an useful tool to find indices for a required application, adapted to a selected sensor.
*  [LandscapeToolbox](https://wiki.landscapetoolbox.org/doku.php/remote_sensing_methods:home) - The Vegetation/Greenness Indices part provides a detailed descriptions and applications of 9 common indices.


## Software programs
There are currently a large number of software with Vegetation Index tools, and we have a brief summary of them, 
### Commercial
|Name|Description|
|--|--|
| ERDAS IMAGINE |  |
| ArcGIS |  |
| ENVI |  |
| Idrisi|  |
### Open Source
|Name|Description|
|--|--|
| QGIS |  |


<!-- End Links (do not remove me) -->

 ## Note

This list will be updated in time, and volunteer contributions are welcome. For questions or sharing, please feel free to  [contact us](mailto:007zhangmin@whu.edu.cn)  or make issues.

