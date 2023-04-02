<a name="page_top"/>  

**Shortcuts** 
|     |    |    |
| --- | ---| ---|
| [![](https://img.shields.io/badge/ML-grey?logo=tensorflow)](#) [1. Machine Learning](#MachineLearning) | [![](https://img.shields.io/badge/CV-grey?logo=opencv)](#) [2. Computer Vision](#ComputerVision)| [![](https://img.shields.io/badge/Cloud-grey?logo=googlecloud)](#) [3. Cloud Computing](#CloudComputing) 
| [![](https://img.shields.io/badge/Image-grey?logo=atom)](#) [4. Image Processing](#ImageProcessing) | [![](https://img.shields.io/badge/Geo-grey?logo=PyG)](#) [5. Geospatial Applications](#GeospatialApp)  | [![](https://img.shields.io/badge/Drone-grey?logo=Drone)](#) [6. Drone/UAV sensing](#Drone) 

<a name="MachineLearning"/>  

## Machine learning

### 1. MODISNN: a dense neural network

Satellite sensors have a liefspan and different configurations. How can we use machine learning to build a consistent product among multiple sensors and create a >20 years time-series dataset for climate change studies?

<table border="0">
 <tr>
  <td>
     Figure 1. The illustration of using nerual network to fill satellite observation gap in 2012-2015 (red question mark)
    <img src="images/modisNN_abstract.png" width="2000">
  </td>
  <td>
     Figure 2. An example of NN model performance at image level (left 2 columns: reference; right 2 columns: nerual network training result)
    <img src="images/modisNN_rst.png?raw=true" width="2000"/>
  </td>
 </tr>
</table>

[![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Jupyter-grey?logo=Jupyter)](#) [![](https://img.shields.io/badge/Tensorflow-grey?logo=Tensorflow)](#) [![](https://img.shields.io/badge/Anaconda-grey?logo=Anaconda)](#) 

[View GitHub Project](https://github.com/chqzeng/MODISNN)  |  [View Publication](https://www.mdpi.com/2072-4292/13/17/3349#)  

<!-- unused: https://pub.mdpi-res.com/remotesensing/remotesensing-13-03349/article_deploy/html/images/remotesensing-13-03349-ag.png?1630051208  the image from publication -->

### 2. AlgaeDriver: assess input features' importance to the output variable  
Use continuous geographic, hydrological, climate, and meteorological datasets as input to train neural network(NN) and random forest(RF) models, to determine the major environmentl drivers of algae growth in lakes.  
Use Google Cloud Platform (GCP) to extract relative data from its [Earth Engine Dataset](https://developers.google.com/earth-engine/datasets) and run further NN models    
Figure 1. The illustration of machine learning model input and output varialbes   
<img src="images/AlgaeDrivers.png" height="400" />   
[View code partially on Github](https://github.com/chqzeng/OpenWL/blob/main/AlgaeDrive/AlgaeDrive.ipynb)  

[![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Jupyter-grey?logo=Jupyter)](#) [![](https://img.shields.io/badge/Tensorflow-grey?logo=Tensorflow)](#) [![](https://img.shields.io/badge/GoogleCloud-grey?logo=GoogleCloud)](#) [![](https://img.shields.io/badge/GEE-grey?logo=googleearth)](#) 

### 3. Coursera Course: "Machine Learning"
<details open >
<summary> View Certificate </summary>   

<img src="materials/Coursera_DL9CTNZK3T6P.png" height="200" />  [view on coursera.org](https://www.coursera.org/account/accomplishments/certificate/DL9CTNZK3T6P)  

</details>

[Back to Top](#page_top)

---
<a name="ComputerVision"/>  

## Computer Vision

### 1. Detect urban objects from high-resolution imagery (2014 work)  

#### A) River channel detection from optical and SAR imagery
Integrated Optical and radar imagery are combined for unsuprevised image classification and then a decision tree to refine the result with unique attributes to sense water.
<table border="0">
 <tr>
  <td>
     Figure 1. An illustration of detection of the Bow River at Calgary, Aberta, CA.  
     (a) input optical (WV-2) image, (b) SAR (RadarSat-2) of the study site, (c) object-based unsupervised classification (b) extracted water mask, (e) optical and SAR combined river channel detection.  
    <img src="images/river_detection2011.png" height="300">
  </td>
  <td>
     Figure 2. An illustration to connect river channel segments and build a topologically-correct river 
     <img src="images/River_seg_connection.png" width="500" />
  </td>
 </tr>
</table>  

[View project code on Github](https://github.com/chqzeng/NRBC)


#### B) Building and tree detection from aerial photo and LiDAR point clouds (2010 work)
From a high resolution (<1m) satellite imagery or aerial photo, detect buildings of varied conditions.

<table border="0">
 <tr>
  <td>
     Figure 1. An illustration of urban building detection from aerial photos and LiDAR point clouds  
    <img src="materials/building_detection.gif" height="500">
  </td>
  <td>
     Figure 2. The reconstructed 3D buildings and trees   
     <img src="materials/campus_3d_buildings.gif" height="500" />
  </td>
 </tr>
</table>  

[Ph.D Dissertation](https://ir.lib.uwo.ca/etd/2076/): "Automated Building Information Extraction and Evaluation from High-resolution Remotely Sensed Data" 


[<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#)  [![](https://img.shields.io/badge/OpenCV-grey?logo=OpenCV)](#) [![](https://img.shields.io/badge/3Dmodel-grey?logo=Sketchup)](#) 

### C) Esitmate image depth and 3D model from mutli-view imagery (2015 work)

[Multi-view image matching to reconstruct the 3D Earth surface](https://www.taylorfrancis.com/chapters/edit/10.1201/9780429470196-5/multiview-image-matching-3d-earth-surface-reconstruction-chuiqing-zeng-jinfei-wang)
[A Stereo Image Matching Method to Improve the DSM Accuracy inside Building Boundaries](http://pubs.casi.ca/doi/abs/10.5589/m13-039)

### D) Image systhesis (2008 work)
systhese two or more imagery into a single imagery with minimal "cost" 
[View Code](#)  

[Back to Top](#page_top)   

---
<a name="CloudComputing"/>  

## Cloud computing

### High perofmrance computering cluster (HPC) development
develop and deploy massive data processing (>100TB) of satellite imagery processing on the HPC system.

### Azure webportal optimization
maintain and optimize the Azure web portal: mostly maintain the Blob /COG imagery and PostgreSQL database optimization.
[View the website](https://eolakewatch-staging.azurewebsites.net/)

<details open>
 <summary>Click Image below to explore EOLakeWatch</summary>  
 
[![EOLakeWatch](images/EOLakeWatch_webapp.png)](https://eolakewatch-staging.azurewebsites.net/webapp/)   
 
</details>


<!-- <iframe src="https://public.tableau.com/views/EOLakeWatchAttentionLacsOTEN/EOLakeWatch-AttentionLacsOT?:toolbar=n&amp;:display_count=y&amp;:origin=viz_share_link?:embed=y&amp;:display_count=yes&amp;:showVizHome=no" width="100%" height="600px"></iframe>
-->
<!-- <img src="images/EOLakeWatch_webapp.png?raw=true"/>  
[Explore EOLakeWatch](https://eolakewatch-staging.azurewebsites.net/webapp/)   -->

---
<a name="ImageProcessing"/> 

## Image processing
### Raster to Vector and topological correction
[A Natural-Rule-Based-Connection (NRBC) Method for River Network Extraction from High-resolution Imagery](http://www.mdpi.com/2072-4292/7/10/14055/html)


---
<a name="GeospatialApp"/> 

## Geospatial Application
### populatoin spatialization
Given an administrative boundary and its total population, how to determine the population spatial distribution within that admin boundary?
[Population spatialization in china based on night-time imagery and land use data](http://www.tandfonline.com/doi/abs/10.1080/01431161.2011.569581)



--- 
<a name="Drone"/> 

## Drone/UAV sensing development
### UAV sensing for agriculture application
Raspebery PI as the control unit to connect multiple sensors on board the quad-rotatory drones

### UAV sensing for water application

[back](./)
