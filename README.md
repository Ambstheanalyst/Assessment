<h2>How-to Guide on calculating the Normalized Difference Vegetation of acquired Landsat imagery as a proxy for assessing vegetative health</h2>

<h3>Introduction</h3>
This How-to Guide demonstrates how to use Python programming language to calculate a study area’s Normalized Difference Vegetation Index from  acquired Landsat imagery. 
<br>
The Normalized Difference Vegetation Index “represents the relation between spectral reflectance and vegetation cover” (Lamyaa, et. al, 2021). Chlorophyll, or the pigment that plants produce in their leaves reflects best in visible light (red) and the actual cell structure of plants reflects best in near-infrared (NASA’s Earth Observatory, 2000). The more leaves a plant has, the more these wavelengths of light are affected, respectively” (NASA’s Earth Observatory, 2000). Therefore, the output of NDVI is a measurement of the density of plants as an indicator of its state of health. Previous studies have used python programming to calculate NDVI and use it as a proxy for assessing vegetative health, such as Lamyaa et. al’s study of desertification in Wadi El-Rayan, Egypt (Lamyaa et. al, 2021), and Szabo et. al’s study of sedimentation-induced vegetation spread resulting in the succession of a Hungarian lake (Szabo et. al, 2020). 
<br>
The code in this How-to Guide is sourced from Hatari Labs’s ‘NDVI calculation from Landsat 8 images with Python 3 and Rasterio’ tutorial. 

<h2>Set-up / Installation</h2>
<br>
Data
Prior to installation and running this code, test data will need to be retrieved. Landsat imagery provided in this How-to Guide is sourced from the USGS EarthExplorer user interface. Frames selected were from 2003 (Landsat 5) – which is prior to the founding of AgroSB Agropecuária SA and building of Lagoa do Triunfo ranch in 2005 and 2021 (Landsat 8) to assess the area’s present day NDVI. 
Rasters were georeferenced and clipped to the same extents using ArcGIS Pro’s Georeferencing and Extract by Mask tools. 
<br>
Modules & Dependencies 
This code uses the following modules and their respective dependences: 
NumPy 
Rasterio with the following dependencies: 
     -Rasterio.plot 
     -Rasterio.features
Matplotlib with the following dependencies: 
     -matplotlib.pyplot
     -matplitlib notebook
     -matplotlib inline 
OS
