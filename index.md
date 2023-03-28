##### **Table of Contents** 
|:-------------|:------------------|
|[1. Machine Learning](#MachineLearning) | [2. Computer Vision](#ComputerVision)  |
| [3. Cloud Computing](#CloudComputing)   | good and plenty   |

 
[1. Machine Learning](#MachineLearning)    

[2. Computer Vision](#ComputerVision)    

[3. Cloud Computing](#CloudComputing)    

[4. Image Processing](#ImageProcessing)  

[5. Geospatial Applications](#GeospatialApp)  

[6. Drone/UAV sensing](#Drone)  


<a name="MachineLearning"/>  

## Machine learning

### modisNN: a Dense Neural Network

Satellite sensors have a lifespan. How can we use machine learning to build a consistent product among multiple sensors and create a >20 years time-series dataset for climate change studies?
<!-- https://pub.mdpi-res.com/remotesensing/remotesensing-13-03349/article_deploy/html/images/remotesensing-13-03349-ag.png?1630051208  the image from publication -->

Figure 1. The illustration of using nerual network to fill satellite observation gap in 2012-2015 (red question mark)
<img src="images/modisNN_abstract.png?raw=true" />

Figure 2. An example of NN model validation at image level (left 2 columns: reference; right 2 columns: nerual network training result)
<img src="images/modisNN_rst.png?raw=true" width="1000"/>

[![](https://img.shields.io/badge/Python-white?logo=Python)](#) [![](https://img.shields.io/badge/Jupyter-white?logo=Jupyter)](#) [![](https://img.shields.io/badge/Tensorflow-white?logo=Tensorflow)](#) [![](https://img.shields.io/badge/Anaconda-white?logo=Anaconda)](#) 

[View GitHub Project](https://github.com/chqzeng/MODISNN)  |  [View Publication](https://www.mdpi.com/2072-4292/11/19/2306)

### AlgaeDrive: machine learning models to determine dominant environmentl drives of algae growth
Use continuous geographic, hydrological, climate, and meteorological datasets as input to train neural network(NN) and random forest(RF) models and determine the major drivers of algae growth in lakes.
Use Google Cloud Platform (GCP) and its [Earth Engine Dataset](https://developers.google.com/earth-engine/datasets) to train further models

[View code partially on Github](https://github.com/chqzeng/OpenWL/tree/main/S2MSI_LST8_chl)

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