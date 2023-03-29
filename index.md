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


[![](https://img.shields.io/badge/Python-white?logo=Python)](#) [![](https://img.shields.io/badge/Jupyter-white?logo=Jupyter)](#) [![](https://img.shields.io/badge/Tensorflow-white?logo=Tensorflow)](#) [![](https://img.shields.io/badge/Anaconda-white?logo=Anaconda)](#) 

[View GitHub Project](https://github.com/chqzeng/MODISNN)  |  [View Publication](https://www.mdpi.com/2072-4292/13/17/3349#)  

<!-- unused: https://pub.mdpi-res.com/remotesensing/remotesensing-13-03349/article_deploy/html/images/remotesensing-13-03349-ag.png?1630051208  the image from publication -->

### 2. AlgaeDrive: assess input features' importance to the output variable  
Use continuous geographic, hydrological, climate, and meteorological datasets as input to train neural network(NN) and random forest(RF) models, to determine the major environmentl drivers of algae growth in lakes.  
Use Google Cloud Platform (GCP) to extract relative data from its [Earth Engine Dataset](https://developers.google.com/earth-engine/datasets) and run further NN models

[View code partially on Github](https://github.com/chqzeng/OpenWL/blob/main/AlgaeDrive/AlgaeDrive.ipynb)  
Figure 1. The illustration of machine learning model input and output varialbes
<img src="images/AlgaeDrivers.png.png?raw=true" width="2000"/>  

[Back to Top](#page_top)

---
<a name="ComputerVision"/>  

## Computer Vision

### detect buildings from high-resolution imagery
from a high resolution (<1m) satellite imagery or aerial photo, detect buildings of varied conditions.

[Automated Building Information Extraction and Evaluation from High-resolution Remotely Sensed Data](https://ir.lib.uwo.ca/etd/2076/)


### esitmate image depth and 3D model from mutli-view imagery

[Multi-view image matching to reconstruct the 3D Earth surface](https://www.taylorfrancis.com/chapters/edit/10.1201/9780429470196-5/multiview-image-matching-3d-earth-surface-reconstruction-chuiqing-zeng-jinfei-wang)
[A Stereo Image Matching Method to Improve the DSM Accuracy inside Building Boundaries](http://pubs.casi.ca/doi/abs/10.5589/m13-039)

### Image systhesis
systhese two or more imagery into a single imagery with minimal "cost" 
[View Code]() 

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
