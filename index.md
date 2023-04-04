<a name="page_top"/>  

**Page Navigation** 
|     |    |    |
| --- | ---| ---|
| [![](https://img.shields.io/badge/ML-grey?logo=tensorflow)](#) [1. Machine Learning](#MachineLearning) | [![](https://img.shields.io/badge/CV-grey?logo=opencv)](#) [2. Computer Vision](#ComputerVision)| [![](https://img.shields.io/badge/Cloud-grey?logo=googlecloud)](#) [3. Cloud Computing](#CloudComputing) 
| [![](https://img.shields.io/badge/Image-grey?logo=atom)](#) [4. Image Processing](#ImageProcessing) | [![](https://img.shields.io/badge/Geo-grey?logo=PyG)](#) [5. Geospatial Applications](#GeospatialApp)  | [![](https://img.shields.io/badge/Drone-grey?logo=Drone)](#) [6. Drone/UAV sensing](#Drone) 

<a name="MachineLearning"/>  

## Machine learning
<details open >  
 
### 1. MODISNN: a dense neural network

Satellite sensors have a liefspan and different configurations. How can we use machine learning to build a consistent product among multiple sensors and create a >20 years time-series dataset for climate change studies?

<table border="0">
 <tr>
  <td>
     Figure 1. The illustration of using nerual network to fill satellite observation gap in 2012-2015 (red)
    <img src="images/MODISNN_illustration.png" width="2000">
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

 <a name="AlgaeDriver"/>  
 
### 2. AlgaeDriver: assess input features' importance to the output variable  
Use continuous geographic, hydrological, climate, and meteorological datasets as input to train neural network(NN) and random forest(RF) models, to determine the major environmentl drivers of algae growth in lakes.  
Use Google Cloud Platform (GCP) to extract relative data from its [Earth Engine Dataset](https://developers.google.com/earth-engine/datasets) and run further NN models    
Figure 1. The illustration of machine learning model input and output varialbes   
<img src="images/AlgaeDrivers.png" height="400" />   
[View code partially on Github](materials/AlgaeDrive.ipynb)  

[![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Jupyter-grey?logo=Jupyter)](#) [![](https://img.shields.io/badge/Tensorflow-grey?logo=Tensorflow)](#) [![](https://img.shields.io/badge/GoogleCloud-grey?logo=GoogleCloud)](#) [![](https://img.shields.io/badge/GEE-grey?logo=googleearth)](#) 

### 3. Coursera Course: "Machine Learning"
<details open >
<summary> View Certificate </summary>   

<img src="materials/Coursera_DL9CTNZK3T6P.png" height="200" />  [view on coursera.org](https://www.coursera.org/account/accomplishments/certificate/DL9CTNZK3T6P)  

</details>

 </details>  
 </br>  
 
[Back to Top](#page_top)


---
<a name="ComputerVision"/>  

## Computer Vision

<details open >  

### 1. Detect urban objects from high-resolution imagery (2014 work)  

#### A) River detection from optical and SAR imagery
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


#### B) Building detection from aerial photo and LiDAR point clouds (2010 work)
From a high resolution (<1m) satellite imagery or aerial photo, detect buildings of varied conditions.

<table border="0">
 <tr>
  <td>
    Figure 1. An illustration of urban building detection from aerial photos and LiDAR point clouds  <BR> 
    <img src="materials/building_detection.gif" height='500'>
  </td>
  <td>
     Figure 2. The reconstructed 3D buildings and trees   <BR> 
     <img src="materials/campus_3d_buildings.gif" />
  </td>
 </tr>
</table>  

[Ph.D Dissertation](https://ir.lib.uwo.ca/etd/2076/): "Automated Building Information Extraction and Evaluation from High-resolution Remotely Sensed Data" 

[<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#)  [![](https://img.shields.io/badge/OpenCV-grey?logo=OpenCV)](#) [![](https://img.shields.io/badge/3Dmodel-grey?logo=Sketchup)](#) 

#### C) Esitmate image depth and 3D model from mutli-view imagery (2015 work)
<table border="0">
 <tr>
  <td>
     Figure 1. An illustration of image matching using edges as constrains<BR>   
    <img src="images/An example of the stereo image matching process.png" width="400" />
  </td>
  <td>
     Figure 2. How intensity and edge match can improve the stero matching reliability <BR>    
     <img src="images/The matching rates for a sample building.png" width="400" />
  </td>
 </tr>
</table>  

[Code in IDL / Matlab](materials/Image_matching.zip)  |  [Journal Paper](https://www.tandfonline.com/doi/abs/10.5589/m13-039)  |  [Book Chapter](https://www.taylorfrancis.com/chapters/edit/10.1201/9780429470196-5/multiview-image-matching-3d-earth-surface-reconstruction-chuiqing-zeng-jinfei-wang)


#### D) Seamless image/video systhesis (2008 work)
seamless synthesis is the process of generate a larger image / longer video based on small images/videos with textures, including single image texture synthesis (2-D), multi-image interactive synthesis(2-D) and video synthesis (3-D). <BR> The main idea was to minimize the energy function at the connection when synthesizing multiple images/frames together.
<table border="0">
 <tr>
  <td width="400">
     An example of single image texture synthesis to create a larger image  <BR> 
    <img src="materials/single_image_syns.jpg" />
  </td>
  <td width="400">
     An example of multi-image interactive synthesis <BR>    
     <img src="materials/river.gif"  />
  </td> 
  <td width="400">
     Another example of multi-image interactive synthesis <BR>    
     <img src="materials/flowers.gif"  />
  </td>
 </tr>
</table>   

[View C++ codes and files](materials/Image_syn_demo.zip)  

</details>  

</br>  

[Back to Top](#page_top) 

---
<a name="CloudComputing"/>  

## Cloud computing
<details open >  

### High perofmrance computering cluster (HPC) 
with the recent [HPC](https://www.canada.ca/en/shared-services/corporate/data-centre-consolidation/high-performance-computing.html) deployed in the Federal Government, I developed and maintain pipeline to process massive data (>100TB) satellite images in real-time. It feeds time-series data to the following Microsoft Azure webportal
 An illustration of HPC structure and major tools used for the data processing pipeline  
<img src="images/HPC_infrastructure.png" height=300 />

### Microsoft Azure 
with an environment mornitoring webportal [EOLakewatch](https://eolakewatch-staging.azurewebsites.net/) deployed on Azure, I maintain the Blob storage/COG imagery and optimize the PostgreSQL database with billions of records.  
 
<img src="images/EOLakeWatch_webapp.png" height=300 />
 
### CREODIAS / Cloudferro 
use CREODIAS Earth Observation (EO) data portal to access 20+ years time series Earth Observation data and direct process without download using Linux virtual machines (VM).  
 
<img src="images/CREODIAS-graph.png" height=250 />
 
### Google Cloud Platform (GCP) 
collect various meteriological and climate data to study Algae growth in lakes using APIs for massive data download from [GEE](https://developers.google.com/earth-engine/datasets/catalog) and [CDS](https://cds.climate.copernicus.eu/cdsapp#!/search?type=dataset). run the processing with GCP virtual machine and manage data in bucket and postprocess to be ready for further machine learning models.   
more details in above [AlgaeDriver](#AlgaeDriver)
</details>  

<br/>   

[Back to Top](#page_top)   

---
<a name="ImageProcessing"/> 

## Image processing

<details >  

To Be Continue
<!-- ### Raster to Vector and topological correction
[A Natural-Rule-Based-Connection (NRBC) Method for River Network Extraction from High-resolution Imagery](http://www.mdpi.com/2072-4292/7/10/14055/html)  
-->

</details>  

<br/>   

[Back to Top](#page_top)  

---
<a name="GeospatialApp"/> 

## Geospatial Application  
<details open>  
 
### populatoin spatialization
Given an administrative boundary and its total population, how to determine the population spatial distribution within that admin boundary?
[Population spatialization in china based on night-time imagery and land use data](http://www.tandfonline.com/doi/abs/10.1080/01431161.2011.569581)
use [nighttime light](https://ngdc.noaa.gov/eog/download.html) and [land use](https://forobs.jrc.ec.europa.eu/products/glc2000/glc2000.php) dataset to determine the spatial distribution of population.
 
<table border="0">
 <tr>
  <td width="600">
     input data 1: land use land cover <BR> 
    <img src="images/landuse_glc2000.png" />
  </td>
  <td width="600">
     input data 2: nighttime light <BR>    
     <img src="images/nightime_ligh_2006nov.png"  />
  </td> 
  </tr>
 
 <tr>
  <td width="600">
     input data 3: population in administrative boundaries <BR>    
     <img src="images/pop_grid_2008_census.png"  />
  </td>
   <td width="600">
     output data: population in 1km grids <BR>    
     <img src="images/pop_grid_2000_spatialized.png"  />
  </td>
 </tr>
 
</table>   
 

<br/>  

[![](https://img.shields.io/badge/SQL-grey?logo=microsoftsqlserver)](#) [<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#) [![](https://img.shields.io/badge/ExcelVBA-grey?logo=microsoftexcel)](#)  [![](https://img.shields.io/badge/ArcGIS-grey)](#)    

[view partial codes](materials/Pop_spatialization.zip)


### Vehicle-based POI collection system 
develop a light platform that can collect and update points of interest (POIs) with vehicle top-mounted cameras and GPS-receiver, to update existing POI database and collect street-view map like Google Street View.
<table border="0">
 <tr>
    <td width="600">
      the illustration of the survey platform <BR>    
     <img src="images/survey_system_illustration.png"  />
  </td> 
     
  <td width="600">
     the survey platform interface with loaded POIs <BR> 
    <img src="images/Interface0.png" />
  </td>
  <td width="600">
     image extracted from vehicle top-mounted camera videos <BR>    
     <img src="images/Camera.png"  />
  </td>
 </tr>
 
</table>  
 
[![](https://img.shields.io/badge/SQL-grey?logo=microsoftsqlserver)](#)  [![](https://img.shields.io/badge/CSharp-grey?logo=CSharp)](#) [![](https://img.shields.io/badge/VisualStudio-grey?logo=visualstudio)](#) [![](https://img.shields.io/badge/GPS-grey)](#)        
 
[view partial codes](materials/Vehicle_based_POI_collection.zip)

</details>  

[Back to Top](#page_top)  

--- 
<a name="Drone"/> 

## Drone/UAV sensing development  

<details>  

### UAV sensing for agriculture application
Raspebery PI as the control unit to connect multiple sensors on board the quad-rotatory drones

 <table border="0">
 <tr>
    <td width="600">
      the illustration of the drone/UAV hardware setup <BR>    
     <img src="images/illustration_drone_work.png"  />
  </td> 
     
  <td width="600">
     an example of UAV flight planning over water<BR> 
    <img src="images/Drone_flight_illustration.png" />
  </td>
 </tr>
  
 
### UAV sensing for water application
 

</details>  

<br/>  

[Back to Top](#page_top)  


<!--  left over

<details open>
<summary>Click Image below to explore EOLakeWatch</summary>  
[![EOLakeWatch](images/EOLakeWatch_webapp.png)](https://eolakewatch-staging.azurewebsites.net/webapp/)   
</details>
-->
<!-- <iframe src="https://public.tableau.com/views/EOLakeWatchAttentionLacsOTEN/EOLakeWatch-AttentionLacsOT?:toolbar=n&amp;:display_count=y&amp;:origin=viz_share_link?:embed=y&amp;:display_count=yes&amp;:showVizHome=no" width="100%" height="600px"></iframe>
-->
<!-- <img src="images/EOLakeWatch_webapp.png?raw=true"/>  
[Explore EOLakeWatch](https://eolakewatch-staging.azurewebsites.net/webapp/)   -->
