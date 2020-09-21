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
Normalized Difference Vegetation Index | NDVI |<img src="/tex/7b35265b8f684b978d6ca258ffc1ee24.svg?invert_in_darkmode&sanitize=true" align=middle width=70.97080154999999pt height=29.40633629999998pt/>|Pigment, Canopy | | [paper](https://scholar.google.com/scholar_lookup?title=Monitoring%20vegetation%20systems%20in%20the%20great%20plains%20with%20erts&author=J.%20W.%20Rouse%20Jr.&author=R.%20Haas&author=J.%20Schell&author=&author=D.%20Deering&publication_year=1974))
The Wide Dynamic Range Vegetation Index|WDRVI | <img src="/tex/600d3c5700a8990dedd0db8bdd9c739a.svg?invert_in_darkmode&sanitize=true" align=middle width=97.1250093pt height=29.223734100000023pt/>
Simple Ratio  | SR| <img src="/tex/bf40c029b602e3b5914dc1e39ff6ea84.svg?invert_in_darkmode&sanitize=true" align=middle width=82.1123193pt height=28.92634470000001pt/> 
Atmospherically Resistant Vegetation Index | ARVI|<img src="/tex/e3fca41f3959180a50953448725694d4.svg?invert_in_darkmode&sanitize=true" align=middle width=182.55683489999998pt height=33.20539859999999pt/> | γ| | 
soil and atmosphere resistant vegetation|SARVI|<img src="/tex/ac5ecd355a60014812bd7622561e17ae.svg?invert_in_darkmode&sanitize=true" align=middle width=255.64816199999999pt height=33.20539859999999pt/> | γ|L | 
modified soil and atmosphere resistant vegetation|MSARVI| <img src="/tex/1ac79f9e0f5ef040f6bd9b7aa9d17af3.svg?invert_in_darkmode&sanitize=true" align=middle width=155.95144455000002pt height=29.40633629999998pt/>| γ| | 
atmosphere effect resistant vegetation|IAVI|<img src="/tex/46dbabc4d1446709aebc8baf1df5f4bf.svg?invert_in_darkmode&sanitize=true" align=middle width=188.19612734999998pt height=43.068412200000004pt/> | γ|L |  
Enhanced Vegetation Index | EVI| <img src="/tex/61e9210e3226c32090f8e2b1ec3536a6.svg?invert_in_darkmode&sanitize=true" align=middle width=219.02142405pt height=29.40633629999998pt/>| C1|L |  
Perpendicular Vegetation Index| PVI|<img src="/tex/029ad02dc1660f94e9ecaf7c4de926a1.svg?invert_in_darkmode&sanitize=true" align=middle width=224.90587845pt height=27.77565449999998pt/> | |M,I | 
Soil Adjusted Vegetation Index| SAVI|<img src="/tex/5bca7c251f1e3ae4a30cc11484930ab4.svg?invert_in_darkmode&sanitize=true" align=middle width=144.15353535pt height=29.40633629999998pt/> | |L| 
Transformed Soil Adjusted Vegetation Index| TSAVI|<img src="/tex/757f0d9a2330f2d3e404e07a51523846.svg?invert_in_darkmode&sanitize=true" align=middle width=138.35006625pt height=33.20539859999999pt/> | |M,L| 
Modified Soil Adjusted Vegetation Index| MSAVI|<img src="/tex/1ac79f9e0f5ef040f6bd9b7aa9d17af3.svg?invert_in_darkmode&sanitize=true" align=middle width=155.95144455000002pt height=29.40633629999998pt/> | |L'| 
Optimized Soil Adjusted Vegetation Index| OSAVI|<img src="/tex/f24b89b73ceec65eccb645f1a7c83fc2.svg?invert_in_darkmode&sanitize=true" align=middle width=87.49485195pt height=29.40633629999998pt/> | |θ| 
generalized soil-adjusted vegetation index| GESAVI|<img src="/tex/28678067ab4a4f8a5c299f5cc7a1b914.svg?invert_in_darkmode&sanitize=true" align=middle width=114.30663254999999pt height=29.40633629999998pt/> | |L,M,Z| 
Global Environmental Monitoring _Index_| GEMI|<img src="/tex/7a9eb9f5eef25e1b1b484dd591220c1b.svg?invert_in_darkmode&sanitize=true" align=middle width=180.15604694999996pt height=29.40633629999998pt/> | |n| 
Chlorophyll Absorption Ratio Index | CARI | <img src="/tex/6814fbbdb6bd7e9fe6fee4aac33c1743.svg?invert_in_darkmode&sanitize=true" align=middle width=179.78853089999998pt height=43.068399000000014pt/>
Modified Chlorophyll Absorption Ratio Index | MCARI | 
Difference Vegetation Index|DVI | <img src="/tex/37176aaac1664b188b90769aee6d30c3.svg?invert_in_darkmode&sanitize=true" align=middle width=92.52015299999998pt height=22.465723500000017pt/>
weighted Difference Vegetation Index|WDVI|<img src="/tex/b6c3a8c8f3af540aa5aad0f4cbdfb4ff.svg?invert_in_darkmode&sanitize=true" align=middle width=130.35106094999998pt height=22.465723500000017pt/>| |L |  
Renormalized Difference Vegetation Index|RDVI|<img src="/tex/2703fbdefba16513b6ba9f4007535acf.svg?invert_in_darkmode&sanitize=true" align=middle width=120.43830809999999pt height=27.780749700000012pt/>

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
Normalized Difference Vegetation Index | NDVI |<img src="/tex/7b35265b8f684b978d6ca258ffc1ee24.svg?invert_in_darkmode&sanitize=true" align=middle width=70.97080154999999pt height=29.40633629999998pt/>|Pigment, Canopy | | [paper](https://scholar.google.com/scholar_lookup?title=Monitoring%20vegetation%20systems%20in%20the%20great%20plains%20with%20erts&author=J.%20W.%20Rouse%20Jr.&author=R.%20Haas&author=J.%20Schell&author=&author=D.%20Deering&publication_year=1974))
Visible-band difference vegetation index |VDVI| <img src="/tex/6142b898de743335344015526d401bbc.svg?invert_in_darkmode&sanitize=true" align=middle width=141.23823285pt height=33.93596579999999pt/>
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
| Improved SAVI with self-adjustment factor L             | MSAVI               | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/>  | Canopy structure      | Qi et al. (1994)                   |
| Modified Triangular Vegetation Index                    | MTVI1,MTVI2         | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/5a0600336d6a0b7e3899a60c45e41dcd.svg?invert_in_darkmode&sanitize=true" align=middle width=769.8091335pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/cb02e136bf17910c7d59e3901d67ae40.svg?invert_in_darkmode&sanitize=true" align=middle width=666.31492455pt height=62.465633999999994pt/></p> | Canopy structure      | Rondeaux et al. (1996)             |
| Renormalized Difference Vegetation Index                | RDVI                | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/41d1e2d41c6c08d05910bd9a2bf16008.svg?invert_in_darkmode&sanitize=true" align=middle width=553.0998231pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/9fde1789972a1d2cf763342053116ba1.svg?invert_in_darkmode&sanitize=true" align=middle width=709.0772188499999pt height=62.465633999999994pt/></p> | Canopy structure      | Huete (1988)                       |
| Spectral Polygon Vegetation Index                       | SPVI                | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/f50594a1d6727c587c977bc4eb6ae13c.svg?invert_in_darkmode&sanitize=true" align=middle width=538.8580361999999pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/837d1b4bbce47b4bb8ae884188514e79.svg?invert_in_darkmode&sanitize=true" align=middle width=678.1549203pt height=62.465633999999994pt/></p> | Canopy structure      | Baret et al. (1989)                |
| Anthocyanin Reflectance Index                           | ARI                 | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/d98b41a5f5dd62600529a1b1b428ccfb.svg?invert_in_darkmode&sanitize=true" align=middle width=696.88426665pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/4cd0f30f63b903449804bf424d5235a9.svg?invert_in_darkmode&sanitize=true" align=middle width=654.4899174pt height=62.465633999999994pt/></p> | Carotenoid content    | Penuelas and Filella (1998)        |
| Carter Stress Index                                     | CSI1,CSI2           | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/ab825baeacabc7898cda9ed6e22f678e.svg?invert_in_darkmode&sanitize=true" align=middle width=568.09832475pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/f00061c085cd891d7976ea55b65abedc.svg?invert_in_darkmode&sanitize=true" align=middle width=630.71899275pt height=55.8902916pt/></p> | Chlorophyll           | Gitelson and Merzlyak (1997)       |
| Leaf Chlorophyll Index                                  | LCI,LIC1,LIC2,LIC3  | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/5bd6defb7c0fd9a81a1ce3c0b5d53c15.svg?invert_in_darkmode&sanitize=true" align=middle width=410.70515309999996pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/bbcc2b8e3f03efc736e5cf2b40e597ac.svg?invert_in_darkmode&sanitize=true" align=middle width=816.75981255pt height=62.465633999999994pt/></p> | Chlorophyll           | Daughtry et al. (2000)             |
| Normalized Phaeophytinization Index                     | NPQI                | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/73c7fdfe7186d84e9358078328cd5c72.svg?invert_in_darkmode&sanitize=true" align=middle width=493.25464155pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/0c67e479c4427084c164ca1093e3c326.svg?invert_in_darkmode&sanitize=true" align=middle width=594.63807645pt height=55.8902916pt/></p> | Chlorophyll           | Guyot et al. (1988)                |
| Red Edge Point                                          | REP                 | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/315f42928984a08727458ea0e0bc5919.svg?invert_in_darkmode&sanitize=true" align=middle width=783.95844945pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/26ab8bad8a8a92f49d0b22fda8722250.svg?invert_in_darkmode&sanitize=true" align=middle width=609.4326496499999pt height=55.8902916pt/></p> | Chlorophyll           | Broge and Leblanc (2000)           |
| Vogelmann Index                                         | VOG1,VOG2,VOG3      | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/a862d4fb71902570b5360ac88629cb06.svg?invert_in_darkmode&sanitize=true" align=middle width=455.4528561pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/ef8d506ed7c68e1a4119f5cbcbf89818.svg?invert_in_darkmode&sanitize=true" align=middle width=674.7281326499999pt height=62.465633999999994pt/></p> | Chlorophyll a         | Blackburn (1998)                   |
| Pigment Specific Simple Ratio for Chl b                 | PSSRb               | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/17c209db2a83bf6b61f65fa6babe769c.svg?invert_in_darkmode&sanitize=true" align=middle width=636.9520344pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/10b7f0739c34f2d2385e0605e29d4022.svg?invert_in_darkmode&sanitize=true" align=middle width=627.0967626pt height=55.8902916pt/></p> | Dry Matter / Lignin   | Serrano et al. (2002)              |
| Normalized Difference Nitrogen Index                    | NDNI                | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/3bc0d19fbede8cdb4f94a923d638f597.svg?invert_in_darkmode&sanitize=true" align=middle width=661.9983645pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/64b020e79e5b6e55e01867243564094d.svg?invert_in_darkmode&sanitize=true" align=middle width=608.58786285pt height=55.8902916pt/></p> | Dry Matter / Pigment  | Zarco-Tejada et al. (2005)         |
| Red-Green Pigment Index                                 | RGI                 | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/36fe9b592dee1332b90a755dac0fdce6.svg?invert_in_darkmode&sanitize=true" align=middle width=626.84931045pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/28d1392de38b25f13ffedca78c545401.svg?invert_in_darkmode&sanitize=true" align=middle width=675.6246749999999pt height=62.465633999999994pt/></p> | Water Content         | Galvão et al. (2005)               |
| Leaf Water Vegetation Index                             | LWVI1,LWVI2         | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/db44f97f29bd9a0ed4104babc3af4596.svg?invert_in_darkmode&sanitize=true" align=middle width=464.4265791pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}<p align="center"><img src="/tex/e2b60503a12342b7d404733167f58f0c.svg?invert_in_darkmode&sanitize=true" align=middle width=638.84328255pt height=55.8902916pt/></p> | Water Content         | Gao (1996)                         |
| Plant Water Index                                       | PWI                 | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/><img src="/tex/e4dbe411f18b746b0c1963a53c49c263.svg?invert_in_darkmode&sanitize=true" align=middle width=517.3424916pt height=24.65753399999998pt/>\frac {1}{2} \cdot [2 \cdot R_{800} + 1 – \sqrt{(2 \cdot R_{800} + 1)^2 – 8 \cdot (R_{800} – R_{670}}$$ | Water Content         | Zarco-Tejada et al. (2003)         |
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

