<a name="page_top"/>  

**Page Navigation** 
|     |    |    |
| --- | ---| ---|
| [![](https://img.shields.io/badge/ML-grey?logo=tensorflow)](#) [1. Machine Learning](#MachineLearning) | [![](https://img.shields.io/badge/CV-grey?logo=opencv)](#) [2. Computer Vision](#ComputerVision)| [![](https://img.shields.io/badge/Cloud-grey?logo=googlecloud)](#) [3. Cloud Computing](#CloudComputing) 
| [![](https://img.shields.io/badge/Image-grey?logo=atom)](#) [4. Image Processing](#ImageProcessing) | [![](https://img.shields.io/badge/Geo-grey?logo=PyG)](#) [5. Geospatial Applications](#GeospatialApp)  | [![](https://img.shields.io/badge/Drone-grey?logo=Drone)](#) [6. Drone/UAV sensing](#Drone) 

<a name="MachineLearning"/>  

## Machine Learning
<details open >  
 
### 1. MODISNN: a dense neural network

Satellite sensors have a liefspan and different configurations. How can we use machine learning to build a consistent product among multiple sensors and create a >20 years time-series dataset for climate change studies?

<table border="0">
 <tr>
  <td>  
    <img src="images/MODISNN_illustration.png" width="2000">  
    Using nerual network to fill satellite observation gap in 2012-2015 (red dash line box)
  </td>
  <td>  
     <img src="images/modisNN_rst.png?raw=true" width="2000"/>  
     An example of NN model performance at image level <BR> 
     left 2 columns: reference image; right 2 columns: nerual network trained result
    
  </td>
 </tr>
</table>

[![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Jupyter-grey?logo=Jupyter)](#) [![](https://img.shields.io/badge/Tensorflow-grey?logo=Tensorflow)](#) [![](https://img.shields.io/badge/Anaconda-grey?logo=Anaconda)](#) 

[View GitHub Project](https://github.com/chqzeng/MODISNN)  |  [View Publication](https://www.mdpi.com/2072-4292/13/17/3349#)  

<!-- unused: https://pub.mdpi-res.com/remotesensing/remotesensing-13-03349/article_deploy/html/images/remotesensing-13-03349-ag.png?1630051208  the image from publication -->

 <a name="AlgaeDriver"/>  
 
### 2. AlgaeDriver: assess input features' importance to the output variable  
Use continuous geographic, hydrological, climate, and meteorological datasets as inputs to train neural network(NN) and random forest(RF) models and determine the major environmentl drivers of algae growth in lakes. <BR>
Use Google Cloud Platform (GCP) to extract relative data from its [Earth Engine](https://developers.google.com/earth-engine/datasets) Dataset and run further NN models    
<br>

<img src="images/AlgaeDrivers.png" height="400" />   <BR>
AlgaeDriver machine learning model input and output variables  

[View jupyter code partially on Github](materials/AlgaeDrive.ipynb)  

[![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Jupyter-grey?logo=Jupyter)](#) [![](https://img.shields.io/badge/Tensorflow-grey?logo=Tensorflow)](#) [![](https://img.shields.io/badge/GoogleCloud-grey?logo=GoogleCloud)](#) [![](https://img.shields.io/badge/GEE-grey?logo=googleearth)](#) 

### 3. Coursera Course: "Machine Learning"
<details open >
<summary> View Certificate </summary>   

<img src="materials/Coursera_DL9CTNZK3T6P.png" height="250" />  [view on coursera.org](https://www.coursera.org/account/accomplishments/certificate/DL9CTNZK3T6P)  

</details>

</details>  

</br>  
 
[Back to Top](#page_top)


---
<a name="ComputerVision"/>  

## Computer Vision

<details open >  

### 1. Detect urban objects from high-resolution imagery  

#### A) Detect rivers from optical and SAR imagery
Exploit the unique attributes of water in optical and radar/SAR images by first integrating both images for unsupervised classification, and then refining the results with a decision tree.  
<table border="0">
 <tr>
  <td>  
     <img src="images/river_detection2011.png" height="300">
     Steps to detect the Bow River at Calgary, Aberta, CA.  <BR>
     (a) input 2m WV-2 optical image, (b) RadarSat-2 SAR image, (c) object-based unsupervised classification, (d) extracted water mask, (e) river channel detection after optical and SAR combined.  
    
  </td>
  <td>
     <img src="images/River_seg_connection.png" width="500" />
     Connect the river channel segments to build a topologically correct river
  </td>
 </tr>
</table>  

[<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#)  [![](https://img.shields.io/badge/OpenCV-grey?logo=OpenCV)](#) [![](https://img.shields.io/badge/ArcGIS-grey)](#) [![](https://img.shields.io/badge/eCognition-grey)](#)  

[View project code on Github](https://github.com/chqzeng/NRBC)


#### B) Building detection from aerial photos and LiDAR point clouds (2012)
Detect buildings under varied scenarios from high-resolution (<1m) satellite images or aerial photos.

<table border="0">
 <tr>
  <td width="400">
    <img src="materials/building_detection.gif" >   <BR> 
    Urban building detection from aerial photos and LiDAR point clouds 
  </td>
  <td width="600">
     <img src="materials/campus_3d_buildings.gif" />  <BR> 
     The reconstructed 3D buildings and trees   
  </td>
 </tr>
</table>  

[Ph.D Dissertation](https://ir.lib.uwo.ca/etd/2076/): "Automated Building Information Extraction and Evaluation from High-resolution Remotely Sensed Data" 

[<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#)  [![](https://img.shields.io/badge/OpenCV-grey?logo=OpenCV)](#) [![](https://img.shields.io/badge/C++-grey)](#) [![](https://img.shields.io/badge/eCognition-grey)](#) [![](https://img.shields.io/badge/3Dmodel-grey?logo=Sketchup)](#) 

#### C) Esitmate image depth and 3D model from mutli-view imagery (2015)
<table border="0">
 <tr>
  <td>  
    <img src="images/An example of the stereo image matching process.png" width="400" />  <BR>  
    An example of image matching using edges as constrains 
  </td>
  <td>  
     <img src="images/The matching rates for a sample building.png" width="400" /> <BR>
      Combined intensity and edge matching improves the stero matching reliability 
  </td>
 </tr>
</table>  

[<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#)   [![](https://img.shields.io/badge/IDL-grey?)](#)

[Code in IDL / Matlab](materials/Image_matching.zip)  |   [Journal Paper](https://www.tandfonline.com/doi/abs/10.5589/m13-039)  |  [Book Chapter](https://www.taylorfrancis.com/chapters/edit/10.1201/9780429470196-5/multiview-image-matching-3d-earth-surface-reconstruction-chuiqing-zeng-jinfei-wang)


#### D) Seamless image/video systhesis (2008)
Seamless synthesis is the process of generating a larger image or longer video based on small images with textures or short videos, e.g. single-image texture synthesis (2D), multi-image interactive synthesis (2D), and video synthesis (3D). The main idea is to minimize the energy function at the connection when synthesizing multiple images or frames together.  

<table border="0">
 <tr>
  <td width="400">
    <img src="materials/single_image_syns.jpg" />  <BR> 
    An example of single image texture synthesis to create a larger image  
  </td>
  <td width="400">
     <img src="materials/river.gif"  />  <BR> 
     An example of multi-image interactive synthesis  
  </td> 
  <td width="400">
     <img src="materials/flowers.gif"  />  <BR> 
     Another example of multi-image interactive synthesis  
  </td>
 </tr>
</table>   

[![](https://img.shields.io/badge/C++-grey)](#)  
[View C++ codes and files](materials/Image_syn_demo.zip)  

</details>  

</br>  

[Back to Top](#page_top) 

---
<a name="CloudComputing"/>  

## Cloud computing
<details open >  

<a name="HPCsection"/> 

### High perofmrance computering (HPC) 
Using the recent [HPC](https://www.canada.ca/en/shared-services/corporate/data-centre-consolidation/high-performance-computing.html) established in the Government of Canada, I developed and maintain pipeline to process >100TB satellite images using massive GPUs and CPUs, which feeds time-series data to the following Microsoft Azure webportal.
 
<img src="images/HPC_infrastructure.png" height=300 />   <BR>
The HPC structure and major tools used for the data processing pipeline   

[![](https://img.shields.io/badge/Bash-grey?logo=gnubash)](#) [![](https://img.shields.io/badge/Anaconda-grey?logo=anaconda)](#) [![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Ubuntu-grey?logo=Ubuntu)](#) [![](https://img.shields.io/badge/Docker-grey?logo=Docker)](#)   [![](https://img.shields.io/badge/Intel-grey?logo=Intel)](#) [![](https://img.shields.io/badge/Nvidia-grey?logo=Nvidia) ](#)

### Microsoft Azure 
with an environment mornitoring webportal [EOLakewatch](https://eolakewatch-staging.azurewebsites.net/) deployed on Azure, I maintain the Blob storage/COG imagery and optimize the PostgreSQL database with billions of records.  
 
<img src="images/EOLakeWatch_webapp.png" height=300 />  

[![](https://img.shields.io/badge/Azure-grey?logo=microsoftazure)](#) [![](https://img.shields.io/badge/PostgreSQL-grey?logo=PostgreSQL)](#) [![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Node.js-grey?logo=nodedotjs) ](#)
 
### CREODIAS / Cloudferro 
use CREODIAS Earth Observation (EO) data portal to access 20+ years time series Earth Observation data and direct process without download using Linux virtual machines (VM).  
 
<img src="images/CREODIAS-graph.png" height=250 />  

[![](https://img.shields.io/badge/Cloudferro-grey)](#)  [![](https://img.shields.io/badge/Jupyter-grey?logo=Jupyter) ](#)[![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/Ubuntu-grey?logo=Ubuntu)](#)
 
### Google Cloud Platform (GCP) 
collect various meteriological and climate data to study Algae growth in lakes using APIs for massive data download from [GEE](https://developers.google.com/earth-engine/datasets/catalog) and [CDS](https://cds.climate.copernicus.eu/cdsapp#!/search?type=dataset). run the processing with GCP virtual machine and manage data in bucket and postprocess to be ready for further machine learning models.   
more details in above [AlgaeDriver](#AlgaeDriver)


</details>  

<br/>   

[Back to Top](#page_top)   

---
<a name="ImageProcessing"/> 

## Image processing

<details open> 

### Water quality mapping from satellite imagery  
Apply statistical and machine learning models to over 20 years' worth of 100+Tb satellite imagery using [HPC](#HPCsection), develop and maintain an image processing pipeline that generates both an archive of time-series daily lake statistics starting from 2002 and processes data in near real-time on a daily basis. The project is expanding to monitor all major lakes in Canada.  

<img src="images/Img_processing_workflow.png" height=400 /> 

[![](https://img.shields.io/badge/Python-grey?logo=Python)](#) [![](https://img.shields.io/badge/QGIS-grey?logo=QGIS)](#) [![](https://img.shields.io/badge/ESAsnap-grey)](#) [![](https://img.shields.io/badge/GDAL-grey)](#) [![](https://img.shields.io/badge/XML-grey)](#) 

[View partial codes](https://github.com/chqzeng/OpenWL) | [View publications](https://www.sciencedirect.com/science/article/pii/S0380133022002660)  


### Image fusion  

Q: With two datasets: one covering spatial details but only having 6 bands(colors), and another measuring sparse points spatially but having >100 bands, how can we estimate a dataset with both rich spatial details and >100 bands?  
A: Use a Bayesian missing data imputation approach to fuse the two dataset.
 
 <table border="0">
 <tr>
    <td width="500">
     <img src="images/Zeng_Ag_UAV_hyperdata_fusion.png"  /> <BR>
     the illustration of mutlspectral and spectrometer datasets fusion
  </td> 
     <td width="400">
     <img src="images/tomatofield_hyper_image_cube.png"  /> <BR>  
     an example of the output hyperspectral dataset   
  </td> 
 </tr>
</table>  

[<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#)  [![](https://img.shields.io/badge/Hyperspectral-grey)](#)   
 
[See codes in Matlab (Generate_Hyperspectral_Image.m)](materials/ImageFusion_MSI.zip)  | [View publication](https://www.mdpi.com/2072-4292/9/7/696)  
 
</details>  

<br/>   

[Back to Top](#page_top)  

---
<a name="GeospatialApp"/> 

## Geospatial Application  
<details open>  
 
### populatoin spatialization  
Q: Given an administrative boundary and its total population, how can we determine the spatial distribution of population within that administrative boundary (e.g. in 1km grids)? 
A: Use [nighttime light](https://ngdc.noaa.gov/eog/download.html) and [land use](https://forobs.jrc.ec.europa.eu/products/glc2000/glc2000.php) dataset to determine the spatial distribution of population.
 
<table border="0">
 <tr>
  <td width="600">
    <img src="images/landuse_glc2000.png" /> <BR> 
    input data 1: land use land cover 
  </td>
  <td width="600">
     <img src="images/nightime_ligh_2006nov.png"/>  <BR> 
     input data 2: nighttime light
  </td> 
  </tr>
 
 <tr>
  <td width="600">
     <img src="images/pop_grid_2008_census.png"  />  <BR> 
     input data 3: population in administrative boundaries 
  </td>
   <td width="600">  
     <img src="images/pop_grid_2000_spatialized.png"  />  <BR> 
     output data: population in 1km grids 
  </td>
 </tr>
 
</table>   
 

<br/>  

[<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#) [![](https://img.shields.io/badge/ExcelVBA-grey?logo=microsoftexcel)](#)  [![](https://img.shields.io/badge/ArcGIS-grey)](#)  [![](https://img.shields.io/badge/SQL-grey?logo=microsoftsqlserver)](#)   

[View partial codes](materials/Pop_spatialization.zip)  |  [View publication](http://www.tandfonline.com/doi/abs/10.1080/01431161.2011.569581)


### Vehicle-based POI collection system 
Develop a lightweight platform that can collect and update points of interest (POIs), with cameras and GPS receivers mounted on vehicle top, to update an existing POI database and collect street-view maps similar to Google Street View.  

<table border="0">
 <tr>
    <td width="600">  
     <img src="images/survey_system_illustration.png"  />  <BR>  
     the illustration of the survey platform 
  </td> 
     
  <td width="600">
    <img src="images/Interface0.png" />  <BR>  
    the survey platform interface with loaded POIs 
  </td>
  <td width="600"> 
     <img src="images/Camera.png"  />  <BR>  
     image extracted from captured videos 
  </td>
 </tr>
 
</table>  
 
  [![](https://img.shields.io/badge/VisualStudio-grey?logo=visualstudio)](#) [![](https://img.shields.io/badge/CSharp-grey?logo=CSharp)](#) [![](https://img.shields.io/badge/GPS-grey)](#) [![](https://img.shields.io/badge/SQL-grey?logo=microsoftsqlserver)](#)        
 
[view partial codes](materials/Vehicle_based_POI_collection.zip)

</details>  

[Back to Top](#page_top)  

--- 
<a name="Drone"/> 

## Drone/UAV sensing 

<details open>  

### UAV sensing over land
Experiment Raspberry Pi as the control unit to connect multiple sensors on board the drones, and post-process multi-view images to generate rich 3D terrain and spectral details.

 <table border="0">
 <tr>
    <td width="600">
     <img src="images/illustration_drone_work.png"  /> <BR> 
     The illustration of the drone/UAV hardware setup    
  </td> 
     
  <td width="300">
    <img src="images/Image_Mosiac_photoscan_view.png" height="300"/>   <BR>
    An example of multi-view drone sensing image matching to generate 3D surface <BR> 
  </td>
 </tr>
</table>  

[![](https://img.shields.io/badge/RaspberryPi-grey?logo=RaspberryPi)](#) [<img src="images/Matlab_Logo_grey.png" width="22" />![](https://img.shields.io/badge/Matlab-grey)](#)  [![](https://img.shields.io/badge/DJI-grey)](#) [![](https://img.shields.io/badge/PhotoScan-grey)](#)

[Toolbox on Github](https://github.com/chqzeng/AWM2CSV)  
 
### UAV sensing over water  
Experiment and validate different water optical measurements using the flexible drone platform.  
 
<table border="0">
 <tr>
  <td width="600">
     an example of UAV flight planning over water<BR> 
    <img src="images/Drone_flight_illustration.png" />
  </td>
   
 <td width="600">
     an example of water spectra at different scenarios<BR> 
    <img src="images/drone_water_views2.png" />
  </td>
     
 </tr>
</table>  

[![](https://img.shields.io/badge/DJIPhantom-grey)](#) [![](https://img.shields.io/badge/RaspberryPi-grey?logo=RaspberryPi)](#)

[View publication](https://www.sciencedirect.com/science/article/abs/pii/S0924271617302666)

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
