# Accessing PGC STAC API in Desktop GIS Software
PGC publishes its Digital Elevation Models (DEMs) as an interactive STAC API. These instructions share how to access these datasets from within common desktop GIS platforms.

The STAC API url is: `https://stac.pgc.umn.edu/api/v1/`

## ArcGIS Pro
ESRI provides [instructions for using STAC endpoints within ArcGIS Pro](https://pro.arcgis.com/en/pro-app/latest/help/data/imagery/introduction-to-stac.htm). We will be demonstrating how to create a connection to the PGC STAC, query the API, and add data to your project. One note: this functionality requires ArcGIS Pro version 3.2 or higher.

1. In the ribbon menu, click Insert, then Connections, then STAC Connections. Select New STAC Connection. 
2. The Create STAC Connection opens. Name the Connection something like PGC STAC, and in the Connection field use the URL: https://stac.pgc.umn.edu/api/v1/
3. In the Catalog Pane, click the triangle beside STACs. Your new STAC API connection should be listed.
4. Right-click the connection and click Explore STAC. In the pane which has just opened, you are able to search and query the collections by a variety of parameters.
Click View Results to see the results of your search, and from the Results, click the `Add Data` icon or simply drag and drop to add items onto the map. Currently, preview iamges do not load in the ArcPro STAC viewer.
5. Once added to your map document, you might have to update the symbology to render the DEMs as expected.


## QGIS
The developers of the STAC Spec provide detailed tutorials for [installing the QGIS STAC API Browser Plugin](https://stacspec.org/en/tutorials/1-install-stac-api-browser-qgis-plugin/) and [using the plugin](https://stacspec.org/en/tutorials/2-intro-to-stac-api-browser-qgis-plugin/). We will give a brief overview here for loading the PGC STAC with the tool.

1. Install the STAC API Browser in QGIS. From the plug-ins , select the STAC API Browser. 
3. When the browser opens, click New under the Connections field. 
4. Name the connection something like PGC STAC, and in the URL field use: https://stac.pgc.umn.edu/api/v1/ . Leave the other fields as they are. If you wish, you can click Test connection to confirm the connection works. 
5. You can browse the various collections within PGC’s STAC Catalog and query it by extent. Click Search to view results. 
6. On the Results page, click View assets to see all the files associated with a catalog entry. Each catalog entry will have 8 associated layers. Visit [our website](https://www.pgc.umn.edu/data/elevation/) for a full description of the layers and metadata.