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

We follow Landsat 7 Handbook and Landsat 8 Handbook respectively for calculating the radiance and then the LST in 1995 and 2015. As for calculating radiance before 2013, we used the Landsat 5 TM images and the formula below to convert the DNs of band 6 to radiance. The header file contains LMAX, LMIN, QCALMIN, QCALMAX, and QCAL information.

![AA4](https://github.com/user-attachments/assets/baf288be-880c-4ffa-94f1-436fe3735763)

As for calculating radiance after 2013, we used the Landsat 8 ETM+ images and the formula below to convert the DNs of band 11 to radiance. The header file contains ML, AL, and QCAL information.

![AA5](https://github.com/user-attachments/assets/98b5f438-b2ac-4896-a94d-72f9fd531c87)

The effective at-satellite temperature might be calculated using the following equation in the second stage. The information of K1 and K2 in 1995 and 2015 is in the header files.

![AA6](https://github.com/user-attachments/assets/08a2d954-83d4-404f-9687-f5d8c4294ea1)

The following equation was used to convert the temperature values 'Kelvin (A)' to 'Degree Celsius (B)

![AA7](https://github.com/user-attachments/assets/ed291028-2055-4ac6-b3b8-41d21d262e90)

# Derivation of NDVI from Landsat Imagery

Basically, Normalized Difference Vegetation Index (NDVI) uses the difference between near-infrared and visible radiation divided by the sum of near-infrared and visible radiation to arrive at plant growth density. Mathematically is written as follows:

![AA8](https://github.com/user-attachments/assets/6ee646b1-6612-462e-bcd5-85795aa7662c)

where VIS is the spectral reflectance of visible red light, and NIR is the spectral reflectance of a region in the near-infrared region.

This index output values are between −1.0 and 1.0. No vegetation is there when the value is 0. The values close to +1 (0.8 - 0.9) indicate the highest green density possibility. Values of 0.1 and below relates to flat area such as barren areas of agriculture, rock, sand, or snow. Values between 0.1 to 0.5 indicate parks, shrubs, and grassland, values above 0.5 represent the tropical rainforest.

# Results

## Change in Land Cover

Land Cover maps and analysis were made and done using GIS and Remote sensing software. Following are the Land use classifications of different periods of time.

![AA9](https://github.com/user-attachments/assets/05f862c1-c4ac-4eee-8fb4-eaa335b5dc38)

![AA10](https://github.com/user-attachments/assets/d187bc3f-db53-4b9c-b53f-5e97dd47cdf4)

![AA11](https://github.com/user-attachments/assets/092e56e7-b448-458c-bcd3-cc584973adc9)

There are two trends shown in the figure: (a) compared with 1995, the built-up area in 2015 increased by 90%; and (b) bare land and vegetation had been replaced by 80% in the past 20 years. Water bodies remained constant.

## Change in Land Surfaces Temperature

![AA12](https://github.com/user-attachments/assets/d843a2c3-88c6-49de-8dba-eba6c607ff3b)

Figure above shows how patterns of LST changed from 1995 to 2015. The LST of the northern part of the southeast island remarkably increased. Meanwhile, LST of the northern marginal area decreased considerably.

![AA13](https://github.com/user-attachments/assets/56ba29b5-cf5b-4aa4-8c8d-d70d87161321)

In general, the LST of the majority area of Denpasar City fell into 22-28°C zone in 1995 (96.59%) and increased to 28-32°C in 2015 (94.72%).

## Change in NDVI

![AA14](https://github.com/user-attachments/assets/88e57731-3af0-445a-a608-d63496430601)

There has been a significant change in the vegetation area in Denpasar in 20 years. In terms of flat area, indicated by red area, there is nearly six kilometers square increased in Denpasar City. For built area, indicated by yellow and orange area, there is over 4 kilometers square increased in the city. Finally, for the green area representing forest, there is a significant decrease of 11 kilometers square.

![AA15](https://github.com/user-attachments/assets/1872cb52-fc99-425b-bba6-e47e2ffc1c24)

Comparison of NDVI Index Area in Denpasar in 1995 and 2015

# Conclusion

Using geospatial approaches, this report examines the effects of land cover and use changes on LST in the Denpasar city from 1995 to 2015. The following conclusions can be drawn: (1) Built-up area has doubled in size, and the area of the water body
 
and vegetation area decreased from 1995 to 2015. (2) In Denpasar, the increased amount of built- up and bare area and the decreased amount of water body and vegetation area led to an increase of areas exposed to the urban heat environment in the study period.

The expansion of built-up area partly contributes to the change of land surface temperature in Indonesia. The shape, material, and other design elements should be considered in the planning of the building to reduce the negative impacts of the UHE. Additionally, planning of increasing green infrastructure areas and concepts like rooftop greening and vertical vegetation should be implemented as well.

# References

- Ahmed, B., 2011. Urban land cover change detection analysis and modeling spatio- temporal Growth dynamics using Remote Sensing and GIS Techniques: A case study of Dhaka, Bangladesh. Master’s Thesis, Erasmus Mundus Program, Universidade Nova de Lisboa (UNL), Lisbon, Portugal.
- ESRI., 2012. ArcGIS® 10 Help; Environmental Systems Research Institute: Redlands, CA, USA, 2012. [online] Available at: <http://help.arcgis.com/en/arcgisdesktop/10.0/help/> [Accessed 21 January 2022].
- Landsat 7 (L7) Data Users Handbook., 2019. National Aeronautics and Space Administration, p.54–55. Landsat Project Science Office at NASA’s Goddard Space Flight Center: Greenbelt, MD, USA. [online] Available at: <https://www.usgs.gov/landsat-missions/landsat-7-data-users-handbook> (Accessed on 27 December 2022).
- Landsat 8 (L8) Data Users Handbook., 2019. National Aeronautics and Space Administration, p.117–120. Landsat Project Science Office at NASA’s Goddard Space Flight Center: Greenbelt, MD, USA. [online] Available at <https://www.usgs.gov/media/files/landsat-8-data-users-handbook> (Accessed on 28 December 2022).
- MacLachlan, A., Biggs, E., Roberts, G. and Boruff, B., 2017. Urbanisation-Induced Land Cover Temperature Dynamics for Sustainable Future Urban Heat Island Mitigation. Urban Science, 1(4), p.38.
- NASA., 2000. Earthobservatory. Measuring Vegetation (NDVI & EVI). Normalized Difference Vegetation Index (NDVI). [online] Available at <https://earthobservatory.nasa.gov/features/MeasuringVegetation/measuring_vegeta tion_2.php> [Accessed 21 January 2022].
- Tosepu, R., Gunawan, J., Effendy, D., Ahmad, L., Lestari, H., Bahar, H. and Asfian, P., 2020. Correlation between weather and Covid-19 pandemic in Jakarta, Indonesia. Science of The Total Environment, 725, p.138436.
- Yan, H., Wang, K., Lin, T., Zhang, G., Sun, C., Hu, X. and Ye, H., 2021. The Challenge of the Urban Compact Form: Three-Dimensional Index Construction and Urban Land Surface Temperature Impacts. Remote Sensing, 13(6), p.1067.


