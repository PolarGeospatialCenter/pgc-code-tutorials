# pgc-code-tutorials

This repo includes tutorials for using [Polar Geospatial Center](https://www.pgc.umn.edu) (PGC) data and tools in geospatial workflows.

## PGC Dynamic STAC API
### What is STAC?
STAC - [Spatio Temporal Asset Catalog](https://stacspec.org/en) is a standard for organizing geospatial data for convenient access. Essentially, it is a set of GeoJSON-formatted metadata describing location and time for geospatial information, with links to the actual data, so tools can query by spatial and temporal filters and retrieve just the data necessary for your project. The [STAC spec website includes useful tutorials](https://stacspec.org/en/tutorials/) for getting familiar with using these data tools.

### Programmatic access to public PGC data
We use the dynamic STAC API to enable queryable access to PGC data products via python or desktop GIS applications. The tutorials in the `dynamic_stac_api` folder in this repo demonstrate basic functionality for interacting with the STAC API using built-in tools for [ArcGIS and QGIS desktop software](./dynamic_stac_api/desktop_gis_stac_access.md) and with a [python jupyter notebook](https://polargeospatialcenter.github.io/pgc-code-tutorials/dynamic_stac_api/web_files/stac_api_demo_workflow.html). 

To jump in directly, the dynamic STAC API link is: [https://stac.pgc.umn.edu/api/v1/](https://stac.pgc.umn.edu/api/v1/)

### The Digital Elevation Model (DEM) data
The STAC API provides access to the public DEM data that PGC produces from high resolution satellite imagery, specifically for the polar regions through the [ArcticDEM](https://www.pgc.umn.edu/data/arcticdem/) and [Reference Elevation Model of Antarctica (REMA)](https://www.pgc.umn.edu/data/rema/) products, as well as a subset of the [EarthDEM](https://www.pgc.umn.edu/data/earthdem/) data for the area around the Great Lakes region. These are continent-scale, high resolution (2m), repeat coverage elevation models published as time-stamped DEM Strips and (mostly) seamless Mosaics. You can find out more about [this elevation data on our website](https://www.pgc.umn.edu/data/elevation/).


