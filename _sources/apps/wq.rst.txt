.. _wq:

Water Quality
=============

Water Quality parameters Chlorophyll, Total Suspended Solids and Colored Dissolved Organic Matter based on Organic Absorption will be provided by EOMAPs proprietary water quality processor Modular Inversion and Processing System (MIP). The processors include sensor independent state-of-the-art algorithms including adjacency correction, coupled atmospheric-in-water retrieval considering all bi-directional aspects from extreme clean to extreme turbid case 2 waters in a physically correct approach.

Access to the thematic application
----------------------------------

From the thematic application page, click on the **Open App** button for the **Water Quality** application.

.. figure:: ../includes/apps_wq2.png
	:figclass: img-border
	:width: 100%

|
A new page with the geobrowser, data collections and processing services associated to the Water Quality application will appear.

.. figure:: ../includes/apps_wq_geobrowser.png
	:figclass: img-border
	:width: 100%

|
Open the 'Processing Services' section by clicking on **Processing Services** on the right-hand side of the geobrowser window:

.. figure:: ../includes/apps_wq_geobrowser2.png
	:figclass: img-border
	:align: center
	:scale: 100%

|
Within the 'Processing Services' section you will find the Water Quality Service in the 'Services' tab, click on the Icon to open the service:

.. image:: ../includes/apps_wq_processingservices.png
	:width: 45%
.. image:: ../includes/apps_wq_processingservice_wq.png
	:width: 45%

|
Select what kind of **EO Data** data you would like to process using the dropdown menu on the top right, so far Water Quality Service only supports Landsat8 and Sentinel2.

.. figure:: ../includes/apps_wq_eodata.png
	:figclass: img-border
	:align: center
	:scale: 90%

|
Zoom to your region of interest and use the **spatial filter** to spatially restrict the list of scenes: Click on the spatial filter symbol (little square) on the left-hand side of the geobrowser and draw a rectangle on the map. 

.. image:: ../includes/apps_wq_spatialfilter1.png
	:width: 14%
.. image:: ../includes/apps_wq_spatialfilter2.png
	:width: 84%

|
Use the **temporal filter** via the time slider at the bottom of the map to restrict the list of scenes temporally:

.. figure:: ../includes/apps_wq_timefilter.png
	:figclass: img-border
	:align: center
	:scale: 100%

|
The list of available scenes is now filtered for your needs. If you identified a scene you would like to process you can add the scene via drag&drop from the scene list on the bottom left to the Water Quality Service:

.. figure:: ../includes/apps_wq_selectdata.png
	:figclass: img-border
	:align: center
	:width: 100%

|
Select **one** of the three available **processing options**: 

.. figure:: ../includes/apps_wq_selectoption.png
	:figclass: img-border
	:align: center
	:scale: 90%

|
Select a **title** for your processing job, e.g. "My first Water Quality Job for Bamako" 

.. figure:: ../includes/apps_wq_jobtitle.png
	:figclass: img-border
	:align: center
	:scale: 90%

|
Now you can **either** click on the **Run Job** button

.. figure:: ../includes/apps_wq_runjob0.png
	:figclass: img-border
	:align: center
	:scale: 150%

|
**OR** you could add more scenes to your job, from the same EO Data collection or you can even add scenes from another collection.
Therefore just change the **EO Data** collection in the dropdown menu on the top right:

.. figure:: ../includes/apps_wq_eodata2.png
	:figclass: img-border
	:align: center
	:scale: 90%

|
Your selected **spatial and temporal filters remain** and you can look for a scene from the other collection. 
If you identified another scene you would like to process can add the scene via drag&drop from the scene list on the bottom left to the Water Quality Service:

.. figure:: ../includes/apps_wq_selectdata2.png
	:figclass: img-border
	:align: center
	:width: 100%

|
If your are satisfied with your scenes and settings click on the **Run Job** button to start the processing.

.. figure:: ../includes/apps_wq_runjob.png
	:figclass: img-border
	:align: center
	:scale: 90%

|
Results
-------

If your processing job finished sucessfully you can click on the **Show results** button.

.. figure:: ../includes/apps_wq_results1.png
	:figclass: img-border
	:align: center
	:scale: 90%

The results of you processing will be shown in the search results list on the bottom left. The following results will be created: 

|
For processing option **Water Quality Parameters - TSS + CHL + CDOM + SWT (LS8 only)**: 

* The water quality data is delivered as 32bit real value GeoTIFF, as well as 8bit scaled and colored GeoTIFF and corresponding metadata XML for each water quality parameter. 
* Furthermoe EOMAP's water quality products are accompanied by the processor's internal quality control mechanisms, resulting in pixel flagging in case of unreliable values. The QUC file indicates the main quality influencing parameter using a specific EOMAP quality coding classification scheme with corresponding grey values (GV), as shown in the following figure:

.. figure:: ../includes/apps_wq_EOMAP_Quality_CODING_table.png
	:figclass: img-border
	:align: center
	:scale: 90%
 
* Overview of files delivered per satellite scene (example):

  * Total Suspended Solids (TSS): *TSS_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, GeoTiff, 8bit scaled
  * Total Suspended Solids (TSS): *TSS_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030_32bit.tif*, GeoTIFF, 32bit
  * Total Suspended Solids (TSS): *TSS_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata
  * Chlorophyll (CHL): *CHL_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, GeoTiff, 8bit scaled
  * Chlorophyll (CHL): *CHL_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030_32bit.tif*, GeoTIFF, 32bit
  * Chlorophyll (CHL): *CHL_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata
  * Colored Dissolved Organic Matter (CDOM): *CDM_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, GeoTiff, 8bit scaled
  * Colored Dissolved Organic Matter (CDOM): *CDM_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030_32bit.tif*, GeoTIFF, 32bit
  * Colored Dissolved Organic Matter (CDOM): *CDM_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata
  * Surface Water Temperature (SWT): *SWT_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, GeoTiff, 8bit scaled
  * Surface Water Temperature (SWT): *SWT_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030_32bit.tif*, GeoTIFF, 32bit
  * Surface Water Temperature (SWT): *SWT_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata
  * Watermask (WMA): *WMA_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, GeoTIFF, 8bit, GV 100 = water, GV 0 = no water
  * Watermask (WMA): *WMA_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata
  * Quality Coding (QUC): *QUC_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, GeoTIFF, 8bit
  * Quality Coding (QUC): *QUC_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata
  * Total Quality (QUT): *QUT_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, GeoTIFF, 8bit
  * Total Quality (QUT): *QUT_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata
  
|
For processing option **Atmospheric Corrected Image**:

* The atmospheric corrected product is delivered as 32bit multi-channel GeoTIFF with corresponding metadata XML file.
* It provides reflectance data instead of scaled radiances or top-of-the atmosphere products and improves satellite imagery by minizing effects of haze and atmospheric aerosols. Reflectance will be delivered as Remote Sensing Reflectance above surface at nadir (RRS0+).
* Overview of files delivered per satellite scene (example):

  * Remote Sensing Reflectance (RRS): *RRS_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.tif*, Multi-channel GeoTiff, 32bit
  * Remote Sensing Reflectance (RRS): *RRS_wq-tep193050_EOMAP_20161122_101338_LSAT8_m0030.xml*, XML, metadata

|
For processing option **all**: Products of both options described above are delivered.

























