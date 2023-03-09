# Awesome Vegetation Index [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
List of reference, applications of common Vegetation Indices for Multi-spectral, hyper-spectral and UAV images. (**contribution are welcome**)

<img src="https://flurosat.com/wp-content/uploads/2018/10/growth-monitoring-e1583902228867.png)" alt="drawing" width="600"/>

## Table of Contents

<!-- Start TOC (do not remove me) -->
- [Literature Reviews](#literature-reviews-for-vi)
- [Multispectral Vegetation Index](#multispectral-vegetation-index)
  - [Broadband Greenness and Cover](#greenness-and-cover)
  - [Other applications for Broadband  images](#other-applications-for-broadband-images)
- [Hyperspectral Vegetation Index](#hyperspectral-egetation-Index)
- [Vegetation Index for UAV images ](#vegetation-index-for-uav-images  )
- [Community](#community)
  - [Learning Materials](#learning-materials)
- [Software](#Software)
  - [Commercial](#Commercials)
  - [Open](#Open)
 
<!-- End TOC (do not remove me) -->

<!-- Start Links (do not remove me) -->
## Literature Reviews for VI
1. Significant Remote Sensing Vegetation Indices: A Review of Developments and Applications ([li et al. 2017](https://www.hindawi.com/journals/js/2017/1353691/))
2. Research on Vegetation Information Extraction from Visible UAV Remote Sensing Images ([yuan et al. 2018](https://ieeexplore.ieee.org/document/8598637))
3. Hyperspectral vegetation indices and their relationships with agricultural crop characteristics([Thenkabail et al.2000](http://apps.webofknowledge.com/full_record.do?product=UA&search_mode=GeneralSearch&qid=8&SID=5AYEOj1lDfu8CskvSSI&page=2&doc=17))
4. Evaluating Multispectral Images and Vegetation Indices for Precision Farming Applications from UAV Images ([Candiago et al. 2015](https://www.mdpi.com/2072-4292/7/4/4026))

## Multispectral Vegetation Index

### Greenness and Cover
Broadband greenness measures the health of vegetation leaf area index (LAI) and canopy chlorophyll density (CCD) vegetation cover, LAI, biomass, growth, and vigor assessment. It is worthy noting that the selection of proper wavebands in hyperspectral data could partly compensate the limitations of some VI formulas.[(Zhao et al.2007)](https://www.sciencedirect.com/science/article/abs/pii/S0924271607000056)
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


### Other Applications for Broadband Images
Name| Abbrev. | Formula | Satellite Example | Sensitivity | Reference
---|---|---|---|---|---
Photochemical Reflectance Index|PRI | <img src="/tex/da789f46d4f08fa3d44f7b2a2deac813.svg?invert_in_darkmode&sanitize=true" align=middle width=65.10317384999999pt height=29.205422400000014pt/> |  WorldView-2 | Light Use
Structure Insensitive Pigment Index|SIPI | <img src="/tex/c2a215dcebfa06ccb8ef007066d49855.svg?invert_in_darkmode&sanitize=true" align=middle width=61.918216799999996pt height=29.205422400000014pt/> |ALI | Light Use
Normalized Difference Nitrogen Index | NDNI | <img src="/tex/af7c4c6a26a48a064f707175ad94b8c5.svg?invert_in_darkmode&sanitize=true" align=middle width=164.6553711pt height=36.825666900000016pt/> | SCIAMACHY| Nitrogen
Plant Senescence Reflectance Index|PSRI | <img src="/tex/0ddd13665dcc6730c60a976040899b44.svg?invert_in_darkmode&sanitize=true" align=middle width=85.70819399999999pt height=27.77565449999998pt/> | LandsatMSS | Dry or Senescent Carbon
Carotenoid Reflectance Index 1|CRI1 | <img src="/tex/57bee3ccf1fda9b067f2e80bb09f178d.svg?invert_in_darkmode&sanitize=true" align=middle width=142.69442384999996pt height=29.190975000000005pt/> | LandsatTM |Carotenoid 
Anthocyanin Reflectance Index 1|ARI1,ARI2 | <img src="/tex/2fa2595c074759d606e3810ed7e5ee53.svg?invert_in_darkmode&sanitize=true" align=middle width=99.47054534999998pt height=27.77565449999998pt/> | LandsatMSS| Anthocyanin 
Normalized Difference Water Index|NDWI |<img src="/tex/261ccd95c17bfe87595e6fd823abdf58.svg?invert_in_darkmode&sanitize=true" align=middle width=70.69687019999999pt height=29.205422400000014pt/>    | MIPAS | Water 
Moisture Stress Index|MSI |<img src="/tex/827dd6ef4d1d8f7e7db2b30fa6c3af22.svg?invert_in_darkmode&sanitize=true" align=middle width=33.099598949999994pt height=29.205422400000014pt/>     | LandsatTM|Water 
Normalized Difference Infrared Index|NDII | <img src="/tex/a3239a6c5752dce1f4cbb971ab3dc77d.svg?invert_in_darkmode&sanitize=true" align=middle width=95.72359499999999pt height=27.77565449999998pt/> | ALI|Water 




## Hyperspectral Vegetation Index
The overall amount and quality of photosynthetic material in vegetation.

| NAME                                                    | INDEX(series)       | FORMULA (sample)                                                                                                                                                                                              | SENSITIVITY           | Reference                          |
|---------------------------------------------------------|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|------------------------------------|
| Improved SAVI with self-adjustment factor L             | MSAVI               | <img src="/tex/a854f6576305fc09f3270c70aa23573c.svg?invert_in_darkmode&sanitize=true" align=middle width=342.26362995pt height=29.424786600000015pt/>                                                                                                       | Canopy structure      | Qi et al. (1994)                   |
| Modified Triangular Vegetation Index                    | MTVI1,MTVI2         | <img src="/tex/2dd52dc2fb8c3b9c2c3a67a830d6248e.svg?invert_in_darkmode&sanitize=true" align=middle width=262.43776349999996pt height=24.65753399999998pt/>                                                                                                                                       | Canopy structure      | Haboudane et al. (2004)            |
| Normalized Difference Vegetation Index                  | gNDVI,hNDVI, etc    | <img src="/tex/e80b0119ed7caadc8a80a63a111c61fb.svg?invert_in_darkmode&sanitize=true" align=middle width=69.76673054999999pt height=28.670654099999997pt/>                                                                                                                                                                                 | Canopy structure      | Rouse et al. (1974)                |
| Optimized Soil Adjusted Vegetation Index                | OSAVI               | <img src="/tex/8151f9fede071b68f6016da05f2b6923.svg?invert_in_darkmode&sanitize=true" align=middle width=126.57611999999997pt height=33.20539859999999pt/>                                                                                                                                       | Canopy structure      | Rondeaux et al. (1996)             |
| Renormalized Difference Vegetation Index                | RDVI                | <img src="/tex/b78bd8c236252dce070dc78a62e98008.svg?invert_in_darkmode&sanitize=true" align=middle width=75.90230835pt height=29.205422400000014pt/>                                                                                                                                                             | Canopy structure      | Rougean and Breon (1995)           |
| Simple Ratio Index                                      | SR,SR705            | <img src="/tex/ad3b07718c6c870f8749203b570684ed.svg?invert_in_darkmode&sanitize=true" align=middle width=31.347054749999995pt height=28.670654099999997pt/>                                                                                                                                                                                             | Canopy structure      | Jordan (1969); Rouse et al. (1979) |
| Soil Adjusted Vegetation Index                          | SAVI,SAVI2          | <img src="/tex/121ae28ef18fec2fad10ccbbfeb05251.svg?invert_in_darkmode&sanitize=true" align=middle width=162.36415304999997pt height=29.205422400000014pt/>                                                                                                                                              | Canopy structure      | Huete (1988)                       |
| Spectral Polygon Vegetation Index                       | SPVI                | <img src="/tex/55e694635e08cdc280f123d77821de48.svg?invert_in_darkmode&sanitize=true" align=middle width=261.98112764999996pt height=24.65753399999998pt/>                                                                                                                                               | Canopy structure      | Vincini et al. (2006)              |
| Thematic Mapper NDVI                                    | tmNDVI              | <img src="/tex/8e8495d88f6f7a5b9827dfa92d0e3a5e.svg?invert_in_darkmode&sanitize=true" align=middle width=257.19882044999997pt height=43.559980199999984pt/>       | Canopy structure      | Rouse et al. (1974)                |
| Transformed Soil Adjusted Vegetation Index              | TSAVI               | <img src="/tex/8934590904d4af05ef5b817edba0542d.svg?invert_in_darkmode&sanitize=true" align=middle width=108.86405805pt height=33.20539859999999pt/>                                                                                                                                            | Canopy structure      | Baret et al. (1989)                |
| Anthocyanin Reflectance Index                           | ARI                 | <img src="/tex/235e41b4434c7f36a0acbff6b9c1bbe5.svg?invert_in_darkmode&sanitize=true" align=middle width=79.04819175pt height=27.77565449999998pt/>                                                                                                                                                                         | Carotenoid content    | Gitelson et al. (2002)             |
| Pigment Specific Simple Ratio for Carotenoids           | PSSRc               | <img src="/tex/6fc699b60189cdbf156d85c36b771b8c.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Carotenoid content    | Blackburn (1998)                   |
| Structural Independent Pigment Index                    | SIPI                | <img src="/tex/c2a215dcebfa06ccb8ef007066d49855.svg?invert_in_darkmode&sanitize=true" align=middle width=61.918216799999996pt height=29.205422400000014pt/>                                                                                                                                                                 | Carotenoid content    | Penuelas and Filella (1998)        |
| Carter Stress Index                                     | CSI1,CSI2           | <img src="/tex/40cf487b46d2774ed3f7c30e9efbf248.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Chlorophyll           | Carter (1994)                      |
| Chlorophyll Absorption Integral                         | CAI,CRI,CRI2        | <img src="/tex/ed9ea289881a0f2af8d78ec3e80e3cb8.svg?invert_in_darkmode&sanitize=true" align=middle width=259.4693277pt height=51.61677179999998pt/> | Chlorophyll           | Oppelt and Mauser (2003)           |
| Gitelson & Merzlyak Index                               | GM1,GM2             | <img src="/tex/41ecb58f2a7800fc4ac71a7044c009d5.svg?invert_in_darkmode&sanitize=true" align=middle width=19.657639649999997pt height=27.77565449999998pt/>                                                                                                                                                                                             | Chlorophyll           | Gitelson and Merzlyak (1997)       |
| Leaf Chlorophyll Index                                  | LCI,LIC1,LIC2,LIC3  | <img src="/tex/2eebcc327f0046e99a0b45ee22fe2e2a.svg?invert_in_darkmode&sanitize=true" align=middle width=65.10317384999999pt height=29.205422400000014pt/>                                                                                                                                                                 | Chlorophyll           | Datt (1999)                        |
| M Locherer Chlorophyll                                  | MLO                 | <img src="/tex/b1583a7fa7628f1aacd70f3e8cbcb717.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Chlorophyll           | unpublished                        |
| Modified Chlorophyll Absorption in Reflectance Index    | MCARI,MCARI1,MCARI2 | <img src="/tex/ef00a36f629f8443a8d1580e58fa214a.svg?invert_in_darkmode&sanitize=true" align=middle width=152.6242773pt height=29.205422400000014pt/>                                                                                                                                                  | Chlorophyll           | Daughtry et al. (2000)             |
| Normalized Phaeophytinization Index                     | NPQI                | <img src="/tex/4af894d6ddc23c61963ca066a2990a21.svg?invert_in_darkmode&sanitize=true" align=middle width=65.10317384999999pt height=29.205422400000014pt/>                                                                                                                                                                 | Chlorophyll           | Barnes (1992)                      |
| Photochemical Reflectance Index                         | PRI                 | <img src="/tex/da789f46d4f08fa3d44f7b2a2deac813.svg?invert_in_darkmode&sanitize=true" align=middle width=65.10317384999999pt height=29.205422400000014pt/>                                                                                                                                                                 | Chlorophyll           | Gamon et al. (1992)                |
| Red Edge Inflection Point                               | REIP1               | <img src="/tex/9cd81f8a3b8f1a3d3940f27ff1015fc9.svg?invert_in_darkmode&sanitize=true" align=middle width=195.87360045pt height=33.20539859999999pt/>                                                                                                        | Chlorophyll           | Guyot et al. (1988)                |
| Red Edge Point                                          | REP                 | <img src="/tex/f2a1ac0882674e642051580982842511.svg?invert_in_darkmode&sanitize=true" align=middle width=249.64058789999999pt height=32.60265690000002pt/>                                                                                                             | Chlorophyll           | Dawson and Curran (1998)           |
| Transformed Chlorophyll Absorption in Reflectance Index | TCARI               | <img src="/tex/ff06dffaf05315729a94df7af877200c.svg?invert_in_darkmode&sanitize=true" align=middle width=285.6696513pt height=29.205422400000014pt/>                                                                                                                 | Chlorophyll           | Haboudane et al. (2002)            |
| Triangular Vegetation Index                             | TVI                 | <img src="/tex/f9861b7dc94831cee995821efe084929.svg?invert_in_darkmode&sanitize=true" align=middle width=269.74373414999997pt height=24.65753399999998pt/>                                                                                                                                       | Chlorophyll           | Broge and Leblanc (2000)           |
| Vogelmann Index                                         | VOG1,VOG2,VOG3      | <img src="/tex/89c374a2c2594e785059dde6796c6bd6.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                    | Chlorophyll           | Vogelmann (1993)                   |
| Zarco-Tejada & Miller                                   | ZTM                 | <img src="/tex/b2f1ecd1eaf25003a154d80072e73916.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Chlorophyll           | Zarco-Tejada et al. (2001)         |
| Pigment Specific Simple Ratio for Chl a                 | PSSRa               | <img src="/tex/5e4cac908ca68d4b99320932116f7248.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Chlorophyll a         | Blackburn (1998)                   |
| Pigment Specific Simple Ratio for Chl b                 | PSSRb               | <img src="/tex/ff0bec92122fa046c708c61442488ff0.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Chlorophyll b         | Blackburn (1998)                   |
| Shortwave Infrared Green Vegetation Index               | SWIRVI              | <img src="/tex/ed8f8c437e85d479a3e6eebad24bbae0.svg?invert_in_darkmode&sanitize=true" align=middle width=328.37389199999996pt height=24.65753399999998pt/>                                                                                                                                      | Dry Matter            | Lobell et al. (2001)               |
| Normalized Difference Lignin Index                      | NDLI                | <img src="/tex/b42b33abec8048d53d923a508ce38aff.svg?invert_in_darkmode&sanitize=true" align=middle width=164.6553711pt height=36.825666900000016pt/>                                                                                                                   | Dry Matter / Lignin   | Serrano et al. (2002)              |
| Normalized Difference Nitrogen Index                    | NDNI                | <img src="/tex/af7c4c6a26a48a064f707175ad94b8c5.svg?invert_in_darkmode&sanitize=true" align=middle width=164.6553711pt height=36.825666900000016pt/>                                                                                                                   | Dry Matter / Nitrogen | Serrano et al. (2002)              |
| Normalized Pigment Chlorophyll Index                    | NPCI                | <img src="/tex/1e9a6f37ebc3fb961fe345f7aa7e3e82.svg?invert_in_darkmode&sanitize=true" align=middle width=65.10317384999999pt height=29.205422400000014pt/>                                                                                                                                                                 | Dry Matter / Pigment  | Penuelas et al. (1994)             |
| Pigment Index                                           | BGI,BRI             | <img src="/tex/5154584857c0cbe3a47417713bedf6aa.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Dry Matter / Pigment  | Zarco-Tejada et al. (2005)         |
| Red-Green Pigment Index                                 | RGI                 | <img src="/tex/f53f3168bacef000f475a5f71bdd1160.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Dry Matter / Pigment  | Zarco-Tejada et al. (2005)         |
| Simple Ratio Pigment Index                              | SRPI                | <img src="/tex/7742b1df63a287bda016e35dcccfa658.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Dry Matter / Pigment  | Penuelas et al. (1995)             |
| Desease Water Stress Index                              | DSWI,DWSI5          | <img src="/tex/72ada0c306a49e59a10deb57761035ac.svg?invert_in_darkmode&sanitize=true" align=middle width=70.69687019999999pt height=29.205422400000014pt/>                                                                                                                                                                  | Water Content         | Galvão et al. (2005)               |
| Leaf Water Vegetation Index                             | LWVI1,LWVI2         | <img src="/tex/2210097ff71024926303251ce61de57b.svg?invert_in_darkmode&sanitize=true" align=middle width=70.69687019999999pt height=29.205422400000014pt/>                                                                                                                                                               | Water Content         | Galvão et al. (2005)               |
| Moisture Stress Index                                   | MSI                 | <img src="/tex/827dd6ef4d1d8f7e7db2b30fa6c3af22.svg?invert_in_darkmode&sanitize=true" align=middle width=33.099598949999994pt height=29.205422400000014pt/>                                                                                                                                                                                    | Water Content         | Hunt et al. (1989)                 |
| Normalized Difference Water Index                       | NDWI                | <img src="/tex/261ccd95c17bfe87595e6fd823abdf58.svg?invert_in_darkmode&sanitize=true" align=middle width=70.69687019999999pt height=29.205422400000014pt/>                                                                                                                                                               | Water Content         | Gao (1996)                         |
| Plant Water Index                                       | PWI                 | <img src="/tex/af25e9f9afd5f1a94ad322cb4467c04c.svg?invert_in_darkmode&sanitize=true" align=middle width=27.5059026pt height=29.205422400000014pt/>                                                                                                                                                                                     | Water Content         | Penuelas et al. (1997)             |
| Simple Ratio Water Index                                | SRWI                | <img src="/tex/4f7dc85f96dc04075d356f7b513fa591.svg?invert_in_darkmode&sanitize=true" align=middle width=33.099598949999994pt height=29.205422400000014pt/>                                                                                                                                                                                    | Water Content         | Zarco-Tejada et al. (2003)         |

## Vegetation Index for UAV images 
With specific camera, UAV images can be used to calculate all kind of hyperspectral and multi-band vegetation index, where RGB only images can be used to calculate following indices.
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

## Community

### Learning Materials

* [Index Database](https://www.indexdatabase.de/) - An Index-Data-Base (IDB) could be an useful tool to find indices for a required application, adapted to a selected sensor.
*  [LandscapeToolbox](https://wiki.landscapetoolbox.org/doku.php/remote_sensing_methods:home) - The Vegetation/Greenness Indices part provides a detailed descriptions and applications of 9 common indices.


## Software programs
There are currently a large number of software with Vegetation Index tools, and we have a brief summary of them, 
### Commercial
|Name|Description| Customed Calculation | Pre definition Indices | Pre definition Satellite |
|--|--|--|--|--|
| ERDAS IMAGINE | |√ | |
| ArcGIS | 15 Image indices are computed from multiband images  |√| 15|
| ENVI | ENVI exposes 27 of these indices which were selected based upon their robustness, scientific basis, and applicability. |√|27|
| Idrisi| A full suite of mathematical and relational modeling tools for deriving new data layers as a function of existing layers. |√ | |
|Pix4Dfields| Dedicated software for agriculture | √|
|opendronemaphttps://opendronemap.org/webodm/|  √| 
### Open Source
|Name|Description| Customed Calculation | Pre definition Indices | Pre definition Satellite |
|--|--|--|--|--|
| QGIS | |√ | |


<!-- End Links (do not remove me) -->

 ## Note

This list will be updated in time, and volunteer contributions are welcome. For questions or sharing, please feel free to  [contact us](isxzl39@gmail.com)  or make issues.

