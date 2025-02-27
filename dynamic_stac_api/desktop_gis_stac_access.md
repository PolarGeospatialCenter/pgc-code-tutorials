# Accessing PGC STAC API in Desktop GIS Software
PGC publishes its Digital Elevation Models (DEMs) as an interactive STAC API. These instructions share how to access these datasets from within common desktop GIS platforms.

The STAC API url is: `https://stac.pgc.umn.edu/api/v1/`

## ArcGIS Pro
ESRI provides [instructions for using STAC endpoints within ArcGIS Pro](https://pro.arcgis.com/en/pro-app/latest/help/data/imagery/introduction-to-stac.htm). We will be demonstrating how to create a connection to the PGC STAC, query the API, and add data to your project. One note: this functionality requires ArcGIS Pro version 3.2 or higher. Since this is a new feature in ArcGIS Pro, there may be unexpected errors or limited functionality compared to other tools. 

1. In the ribbon menu, click Insert, then Connections, then STAC Connections. Select New STAC Connection.
2. The Create STAC Connection panel opens. Name the Connection something like PGC DEM STAC, and in the Connection field use the URL: https://stac.pgc.umn.edu/api/v1/
3. In the Catalog Pane, click the triangle beside STACs. Your new STAC API connection should be listed.
4. Right-click the connection and click Explore STAC. In the pane which has just opened, you are able to search and query the collections by a variety of parameters.
Click View Results to see the results of your search, and from the Results, click the `Add Data` icon or simply drag and drop to add items onto the map. Currently, preview iamges do not load in the ArcPro STAC viewer.
5. Once added to your map document, you might have to update the symbology to render the DEMs as expected, such as applying a Min/Max or Clip stretch to the DEM symbology layer. 


## QGIS
The developers of the STAC Spec provide detailed tutorials for [installing the QGIS STAC API Browser Plugin](https://stacspec.org/en/tutorials/1-install-stac-api-browser-qgis-plugin/) and [using the plugin](https://stacspec.org/en/tutorials/2-intro-to-stac-api-browser-qgis-plugin/). We will give a brief overview here for loading data from the PGC STAC with the plugin.

1. Install the STAC API Browser in QGIS: from the Plugins menu, search for and select the STAC API Browser, then click `Install Plugin`. 

<img src="./img/qgis_plugins_menu.png" width="50%" height="50%">
<img src="./img/qgis_install_plugin.png" width="50%" height="50%">

2. Launch the plugin by selecting it from the Plugins menu or click on the STAC Browser icon in the toolbar.

<img src="./img/qgis_launch_plugin.png" width="50%" height="50%">

3. When the browser opens, click New under the Connections field.

4. Name the connection something like PGC STAC, and in the URL field use: https://stac.pgc.umn.edu/api/v1/ . Leave the other fields as they are. If you wish, you can click Test connection to confirm the connection works.

<img src="./img/qgis_add_connection.png" width="50%" height="50%">

5. Once you have added the PGC dem STAC connection, click on the `Fetch collections` button to browse the various collections within PGC’s STAC Catalog. Select on use the query options to filter by date or extent. Click Search to view results. 

<img src="./img/qgis_iceland_filter.png" width="50%" height="50%">

6. On the Results page, click View assets to see all the files associated with an item. For Strip DEMs, each item will have 8 associated layers, including the 2m DEM, a 10m hillshade for visualization/preview, and a datamask to remove bad data from the DEM. Visit [our website](https://www.pgc.umn.edu/data/elevation/) for a full description of the layers and metadata.

<img src="./img/qgis_preview_add_assets.png" width="50%" height="50%">