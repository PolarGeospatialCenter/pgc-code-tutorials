# pgc-code-tutorials

This repo includes tutorials for using [Polar Geospatial Center](https://www.pgc.umn.edu) (PGC) data and tools in geospatial workflows.

## PGC Dynamic STAC API
### What is STAC?
STAC - [Spatio Temporal Asset Catalog](https://stacspec.org/en) is a standard for organizing geospatial data for convenient access. Essentially, it is a set of GeoJSON-formatted metadata describing location and time for geospatial information, with links to the actual data, so tools can query by spatial and temporal filters and retrieve just the data necessary for your project. The [STAC spec website includes useful tutorials](https://stacspec.org/en/tutorials/) for getting familiar with using these data tools.

### Programmatic access to public PGC data
We use the dynamic STAC API to enable queryable access to PGC data products via python or desktop GIS applications. The tutorials in the `dynamic_stac_api` folder demonstrate basic functionality for interacting with the STAC API using python, ArcGIS, and QGIS tools. To jump in directly, the dynamic STAC API link is: https://stac.pgc.umn.edu/api/v1/

#### PGC Tutorials
- [Python Jupyter Notebook Workflow Tutorial](./dynamic_stac_api/web_files/stac_api_demo_workflow.html)
- [ArcGIS Pro and QGIS Desktop Tutorials](./dynamic_stac_api/web_files/desktop_gis_stac_access.html.html)

### The Digital Elevation Model (DEM) data
PGC produces DEMs from high resolution satellite imagery and makes them publicly available for the polar regions through the [ArcticDEM](https://www.pgc.umn.edu/data/arcticdem/) and [Reference Elevation Model of Antarctica (REMA)](https://www.pgc.umn.edu/data/rema/) products, as well as a subset of the [EarthDEM](https://www.pgc.umn.edu/data/earthdem/) data for the area around the Great Lakes region that is publicly available. These are continent-scale, high resolution (2m), repeat coverage elevation models published as time-stamped DEM Strips and (mostly) seamless Mosaics. You can find out more about [this elevation data on our website](https://www.pgc.umn.edu/data/elevation/).


