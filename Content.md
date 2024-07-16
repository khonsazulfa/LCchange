# Introduction

The objective of this report is to summarize the change of land cover and use by using the Land Cover Maps and NDVI index in Denpasar in 1995 and 2015 and to analyze their impacts on land surface temperature in this area.

![AA1](https://github.com/user-attachments/assets/5baf360f-bb2a-4763-b33b-8556084cca17)

This study focuses on the context of Denpasar, the capital and main hub of Bali province in Indonesia. Denpasar is in Southern Hemisphere. Around 900 thousand people live in this city with a total land area of 124 km2. The population has boosted approximately 4 times in the past 30 years. The rapid urbanization of Denpasar will significantly impact the change of land cover, which in turn will cause changes in the urban micro-climate. 

# Data Collection

We downloaded Land satellite images (1995 and 2015) from the (US Geological Survey (USGS))[https://www.usgs.gov/] official website to achieve the research purpose. The World Geodetic System (WGS) and Universal Transverse Mercator (UTM) projection (within Zone 50 North)—1984 datum was applied to the images. And the images were acquired in two different years and 20 years apart with pixel sizes of 30 × 30 m.

![AA2](https://github.com/user-attachments/assets/e1941236-b1e8-4efd-8a38-d9b6a4e195f9)

Four land cover types were classified from the acquired satellite images (1995 and 2015)

![AA3](https://github.com/user-attachments/assets/25e12c8e-ce96-4e4e-b629-979b855ca9c4)

# Retrieval of Land Surface Temperature

We follow Landsat 7 Handbook and Landsat 8 Handbook respectively for calculating the radiance and then the LST in 1995 and 2015. As for calculating radiance before 2013, we used the Landsat 5 TM images and the Formula (1) to convert the DNs of band 6 to radiance. The header file contains LMAX, LMIN, QCALMIN, QCALMAX, and QCAL information (Landsat 7 Handbook, 2019).


