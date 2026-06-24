# Awesome Python Geospatial

A curated guide to Python tools, data, learning resources, and standards for maps, GIS, cartography, Earth observation, remote sensing, spatial analysis, and location-aware applications.

## Contents

- [Start Here](#start-here)
- [Core Geospatial Stack](#core-geospatial-stack)
- [Vector Data](#vector-data)
- [Raster and Gridded Data](#raster-and-gridded-data)
- [Interactive Maps and Visualization](#interactive-maps-and-visualization)
- [Spatial Analysis](#spatial-analysis)
- [OpenStreetMap and Networks](#openstreetmap-and-networks)
- [Earth Observation and Remote Sensing](#earth-observation-and-remote-sensing)
- [Cloud-Native Geospatial](#cloud-native-geospatial)
- [Databases and Big Data](#databases-and-big-data)
- [Data Engineering and Orchestration](#data-engineering-and-orchestration)
- [Machine Learning and GeoAI](#machine-learning-and-geoai)
- [3D, Point Clouds, and Terrain](#3d-point-clouds-and-terrain)
- [Web Maps and APIs](#web-maps-and-apis)
- [Command Line Tools](#command-line-tools)
- [Datasets and Data Portals](#datasets-and-data-portals)
- [Learning Resources](#learning-resources)
- [Standards and Formats](#standards-and-formats)
- [Communities and News](#communities-and-news)

## Start Here

- [GeoPandas](https://geopandas.org/) - The main entry point for tabular vector GIS workflows in Python.
- [Shapely](https://shapely.readthedocs.io/) - Geometry objects, predicates, measurements, and constructive geometry operations.
- [pyproj](https://pyproj4.github.io/pyproj/stable/) - Coordinate reference systems, transformations, and geodesic calculations.
- [Rasterio](https://rasterio.readthedocs.io/) - Read, write, window, reproject, and process raster data.
- [Xarray](https://docs.xarray.dev/) - Labeled N-dimensional arrays for climate, ocean, weather, and other gridded datasets.
- [Folium](https://python-visualization.github.io/folium/) - Build Leaflet maps from Python.
- [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) - Publication-quality maps with Matplotlib.
- [PySAL](https://pysal.org/) - Spatial statistics, spatial econometrics, and regional analytics.
- [OSMnx](https://osmnx.readthedocs.io/) - Download, model, analyze, and visualize OpenStreetMap street networks and features.
- [Leafmap](https://leafmap.org/) - Interactive mapping and geospatial analysis in Jupyter and web apps.

## Core Geospatial Stack

- [GDAL](https://gdal.org/) - Foundational raster/vector translation and processing library used throughout the geospatial ecosystem.
- [PROJ](https://proj.org/) - Cartographic projections and coordinate transformations.
- [GEOS](https://libgeos.org/) - Geometry engine behind many topology operations.
- [Fiona](https://fiona.readthedocs.io/) - Pythonic vector file I/O built on GDAL/OGR.
- [pyogrio](https://pyogrio.readthedocs.io/) - Fast vector I/O for GeoPandas using GDAL/OGR.
- [GeoArrow](https://geoarrow.org/) - Columnar geospatial data specification for Arrow-native workflows.
- [Apache Arrow](https://arrow.apache.org/) - Columnar memory format increasingly used for efficient geospatial interchange.
- [NumPy](https://numpy.org/) - Core numerical arrays.
- [pandas](https://pandas.pydata.org/) - Tabular data analysis.
- [SciPy](https://scipy.org/) - Scientific computing primitives used by many spatial libraries.

## Vector Data

- [GeoPandas](https://geopandas.org/) - Spatial extension of pandas with geometry columns.
- [Shapely](https://shapely.readthedocs.io/) - Geometry manipulation and analysis.
- [Fiona](https://fiona.readthedocs.io/) - Read and write formats such as GeoPackage, Shapefile, and GeoJSON.
- [pyogrio](https://pyogrio.readthedocs.io/) - High-performance vector reads and writes.
- [mapclassify](https://pysal.org/mapclassify/) - Choropleth classification schemes.
- [rtree](https://rtree.readthedocs.io/) - Spatial indexing via libspatialindex.
- [h3-py](https://uber.github.io/h3-py/) - Python bindings for Uber's H3 hexagonal spatial index.
- [s2sphere](https://github.com/sidewalklabs/s2sphere) - Python implementation of the S2 spherical geometry library.
- [mercantile](https://mercantile.readthedocs.io/) - Web Mercator tile utilities.
- [morecantile](https://developmentseed.org/morecantile/) - Tile matrix set definitions beyond Web Mercator.
- [geopy](https://geopy.readthedocs.io/) - Geocoding client library.
- [timezonefinder](https://github.com/jannikmi/timezonefinder) - Fast timezone lookup from coordinates.

## Raster and Gridded Data

- [Rasterio](https://rasterio.readthedocs.io/) - Raster I/O and processing.
- [rioxarray](https://corteva.github.io/rioxarray/stable/) - Rasterio-powered geospatial extension for Xarray.
- [Xarray](https://docs.xarray.dev/) - Labeled multidimensional arrays.
- [MetPy](https://arm.columbia.edu/metpy/) - A collection of tools in Python for reading, visualizing, and performing calculations with weather data.
- [Dask](https://docs.dask.org/) - Parallel and out-of-core array/dataframe computation.
- [Zarr](https://zarr.readthedocs.io/) - Chunked, compressed N-dimensional arrays for cloud and local storage.
- [rasterstats](https://pythonhosted.org/rasterstats/) - Zonal statistics over raster data.
- [xarray-spatial](https://xarray-spatial.org/) - Raster and terrain analytics using Xarray-compatible arrays.
- [rio-cogeo](https://cogeotiff.github.io/rio-cogeo/) - Cloud Optimized GeoTIFF creation and validation.
- [rio-tiler](https://cogeotiff.github.io/rio-tiler/) - Read raster tiles from COGs and other sources.
- [rio-mbtiles](https://github.com/mapbox/rio-mbtiles) - Export rasters to MBTiles.
- [verde](https://www.fatiando.org/verde/latest/) - Processing, gridding, and interpolation for spatial data.
- [xESMF](https://xesmf.readthedocs.io/) - Regridding for geospatial and climate datasets.

## Interactive Maps and Visualization

- [Folium](https://python-visualization.github.io/folium/) - Leaflet maps generated from Python.
- [ipyleaflet](https://ipyleaflet.readthedocs.io/) - Interactive Leaflet widgets for Jupyter.
- [Leafmap](https://leafmap.org/) - High-level interactive mapping, Earth Engine helpers, STAC helpers, and raster/vector tools.
- [geemap](https://geemap.org/) - Google Earth Engine workflows in Python and Jupyter.
- [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) - Matplotlib-based cartography.
- [Contextily](https://contextily.readthedocs.io/) - Add tiled basemaps to GeoPandas/Matplotlib plots.
- [GeoViews](https://geoviews.org/) - Geographic visualization built on HoloViews.
- [hvPlot](https://hvplot.holoviz.org/) - High-level plotting for pandas, GeoPandas, Xarray, and Dask.
- [geoplot](https://geoplot.readthedocs.io/) - High-level geospatial plotting for GeoPandas.
- [Datashader](https://datashader.org/) - Render very large point, line, raster, and polygon datasets.
- [Bokeh](https://docs.bokeh.org/) - Interactive browser visualizations from Python.
- [Plotly](https://plotly.com/python/maps/) - Interactive map charts and Mapbox/MapLibre-backed layers.
- [pydeck](https://deckgl.readthedocs.io/) - Python bindings for deck.gl.
- [Lonboard](https://developmentseed.org/lonboard/) - Fast interactive maps for GeoPandas, GeoArrow, and large vector datasets.
- [kepler.gl for Jupyter](https://docs.kepler.gl/docs/keplergl-jupyter) - Visual exploration of large geospatial datasets.

## Spatial Analysis

- [PySAL](https://pysal.org/) - Spatial analysis ecosystem.
- [libpysal](https://pysal.org/libpysal/) - Spatial weights, example datasets, and core PySAL utilities.
- [esda](https://pysal.org/esda/) - Exploratory spatial data analysis.
- [spreg](https://pysal.org/spreg/) - Spatial regression.
- [mgwr](https://pysal.org/notebooks/model/mgwr/intro.html) - Multiscale geographically weighted regression.
- [segregation](https://pysal.org/segregation/) - Spatial segregation measures.
- [momepy](https://docs.momepy.org/) - Urban morphology analysis.
- [PyGeodesy](https://github.com/pypa/geodesy) - Geodetic and geodesic calculations.
- [MovingPandas](https://movingpandas.org/) - Trajectory data analysis.
- [scikit-mobility](https://scikit-mobility.github.io/scikit-mobility/) - Human mobility analysis.
- [Tobler](https://pysal.org/tobler/) - Areal interpolation and dasymetric mapping.
- [GeoStat-Framework](https://geostat-framework.readthedocs.io/) - Geostatistics, random fields, variograms, and kriging.
- [GSTools](https://geostat-framework.readthedocs.io/projects/gstools/) - Spatial random fields and geostatistical tools.
- [PyKrige](https://geostat-framework.readthedocs.io/projects/pykrige/) - Kriging interpolation.
- [scikit-gstat](https://scikit-gstat.readthedocs.io/) - Variogram analysis.

## OpenStreetMap and Networks

- [OSMnx](https://osmnx.readthedocs.io/) - Street networks, routing graphs, and OSM feature downloads.
- [Pyrosm](https://pyrosm.readthedocs.io/) - Read OpenStreetMap PBF files into GeoDataFrames.
- [osmium-tool](https://osmcode.org/osmium-tool/) - Command line OSM data processing.
- [pyosmium](https://docs.osmcode.org/pyosmium/latest/) - Python bindings for osmium.
- [NetworkX](https://networkx.org/) - Graph algorithms used in many network workflows.
- [Pandana](https://udst.github.io/pandana/) - Network accessibility analysis.
- [OSM2Pandas](https://github.com/iamtekson/osm2pandas) - Convert OSM data into pandas/GeoPandas-friendly tables.
- [OpenRouteService Python](https://openrouteservice-py.readthedocs.io/) - Client for routing, isochrones, and geocoding.

## Earth Observation and Remote Sensing

- [Google Earth Engine Python API](https://developers.google.com/earth-engine/guides/python_install) - Planetary-scale geospatial analysis with Earth Engine.
- [geemap](https://geemap.org/) - Pythonic Earth Engine visualization and analysis.
- [Sentinel Hub Python](https://sentinelhub-py.readthedocs.io/) - Client for Sentinel Hub services and satellite data.
- [eo-learn](https://eo-learn.readthedocs.io/) - Earth observation processing pipelines.
- [TorchGeo](https://torchgeo.readthedocs.io/) - PyTorch datasets, samplers, transforms, and models for geospatial ML.
- [Raster Vision](https://docs.rastervision.io/) - Deep learning workflows for geospatial imagery.
- [GeoWombat](https://geowombat.readthedocs.io/) - Raster processing with Xarray and Dask.
- [Satpy](https://satpy.readthedocs.io/) - Read, manipulate, and visualize meteorological satellite data.
- [Herbie](https://herbie.readthedocs.io/) - Download numerical weather prediction model data.
- [cfgrib](https://github.com/ecmwf/cfgrib) - Read GRIB files as Xarray datasets.
- [xcube](https://xcube.readthedocs.io/) - Earth observation data cubes.
- [Open Data Cube](https://www.opendatacube.org/) - Large-scale EO data cube infrastructure.
- [xarray-sentinel](https://github.com/bopen/xarray-sentinel) - Sentinel data access using Xarray.

## Cloud-Native Geospatial

- [Cloud Optimized GeoTIFF](https://www.cogeo.org/) - HTTP-range-friendly GeoTIFF pattern.
- [SpatioTemporal Asset Catalog](https://stacspec.org/) - Catalog standard for geospatial assets.
- [PySTAC](https://pystac.readthedocs.io/) - Create and validate STAC catalogs.
- [pystac-client](https://pystac-client.readthedocs.io/) - Search STAC APIs from Python.
- [stackstac](https://stackstac.readthedocs.io/) - Turn STAC items into Dask-backed Xarray arrays.
- [odc-stac](https://odc-stac.readthedocs.io/) - Load STAC data into Xarray using Open Data Cube conventions.
- [kerchunk](https://fsspec.github.io/kerchunk/) - Virtual references for cloud-friendly access to archival formats.
- [fsspec](https://filesystem-spec.readthedocs.io/) - Filesystem abstraction for local, cloud, and HTTP storage.
- [s3fs](https://s3fs.readthedocs.io/) - S3 filesystem interface for Python.
- [TiTiler](https://developmentseed.org/titiler/) - Dynamic tiling service for COGs and STAC assets.
- [MosaicJSON](https://developmentseed.org/mosaicjson-spec/) - Specification for mosaics of tiled assets.

## Databases and Big Data

- [PostGIS](https://postgis.net/) - Spatial extension for PostgreSQL.
- [GeoAlchemy2](https://geoalchemy-2.readthedocs.io/) - Spatial extension for SQLAlchemy.
- [psycopg](https://www.psycopg.org/psycopg3/docs/) - PostgreSQL adapter for Python.
- [DuckDB Spatial](https://duckdb.org/docs/stable/core_extensions/spatial/overview.html) - Local analytical SQL with spatial types and functions.
- [Apache Sedona](https://sedona.apache.org/) - Distributed geospatial processing on Spark, Flink, and Snowflake.
- [Dask-GeoPandas](https://dask-geopandas.readthedocs.io/) - Partitioned GeoPandas operations with Dask.
- [SpatialPandas](https://github.com/holoviz/spatialpandas) - Columnar vector geometry arrays for scalable visualization.
- [GeoParquet](https://geoparquet.org/) - Cloud-friendly columnar vector format.
- [Ibis](https://ibis-project.org/) - Portable dataframe-style API for SQL engines.
- [GeoMesa](https://www.geomesa.org/) - Distributed spatiotemporal database tooling.

## Data Engineering and Orchestration

- [Apache Airflow](https://airflow.apache.org/) - Platform to programmatically author, schedule and monitor workflows.
- [Dagster](https://dagster.io/) - Orchestration tool for data assets.
- [dbt](https://www.getdbt.com/) - Analytics engineering using SQL.

## Machine Learning and GeoAI

- [scikit-learn](https://scikit-learn.org/) - General machine learning toolkit widely used with spatial features.
- [XGBoost](https://xgboost.readthedocs.io/) - Gradient boosting for structured data.
- [PyTorch](https://pytorch.org/) - Deep learning framework.
- [TorchGeo](https://torchgeo.readthedocs.io/) - Geospatial datasets and training utilities for PyTorch.
- [Raster Vision](https://docs.rastervision.io/) - Deep learning workflows for geospatial imagery.
- [Solaris](https://github.com/CosmiQ/solaris) - Deep learning library for geospatial data.
- [Segmentation Models PyTorch](https://smp.readthedocs.io/) - Semantic segmentation models useful for remote sensing.
- [Albumentations](https://albumentations.ai/docs/) - Image augmentation library commonly used for remote sensing.
- [srai](https://kraina-ai.github.io/srai/) - Spatial representations for AI workflows.
- [GeoSAM](https://github.com/aliaksandr960/GeoSAM) - Segment Anything workflows for geospatial imagery.
- [Open-CD](https://github.com/likyoo/open-cd) - Change detection toolbox.
- [TorchSat](https://github.com/sshuair/torchsat) - PyTorch tools for satellite imagery.
- [DeepForest](https://deepforest.readthedocs.io/) - Tree crown detection from aerial imagery.

## 3D, Point Clouds, and Terrain

- [PDAL](https://pdal.io/) - Point cloud data translation and processing.
- [laspy](https://laspy.readthedocs.io/) - Read and write LAS/LAZ point cloud files.
- [Open3D](https://www.open3d.org/docs/latest/) - 3D data processing and visualization.
- [PyVista](https://docs.pyvista.org/) - 3D plotting and mesh analysis.
- [py3dtiles](https://py3dtiles.org/) - Read and write 3D Tiles.
- [pyvista-xarray](https://github.com/pyvista/pyvista-xarray) - Xarray accessors for PyVista.
- [Whitebox Workflows for Python](https://www.whiteboxgeo.com/manual/wbw-user-manual/book/python_scripting.html) - Terrain, hydrology, and raster/vector geoprocessing.
- [richdem](https://github.com/r-barnes/richdem) - Terrain analysis and hydrologic processing.
- [GemGIS](https://gemgis.readthedocs.io/) - Spatial data processing for geomodeling.

## Web Maps and APIs

- [FastAPI](https://fastapi.tiangolo.com/) - Build Python APIs for geospatial services.
- [Django REST framework GIS](https://github.com/openwisp/django-rest-framework-gis) - GeoJSON support for Django REST framework.
- [django.contrib.gis](https://docs.djangoproject.com/en/stable/ref/contrib/gis/) - Django's geospatial framework.
- [TiTiler](https://developmentseed.org/titiler/) - FastAPI-based dynamic raster tiler.
- [Martin](https://maplibre.org/martin/) - Vector tile server for PostGIS and MBTiles.
- [Tegola](https://tegola.io/) - Vector tile server.
- [MapLibre GL JS](https://maplibre.org/maplibre-gl-js/docs/) - Open-source web map renderer.
- [Leaflet](https://leafletjs.com/) - Lightweight interactive web maps.
- [OpenLayers](https://openlayers.org/) - Feature-rich browser mapping library.
- [deck.gl](https://deck.gl/) - GPU-accelerated large-scale geospatial visualization.

## Command Line Tools

- [GDAL command line programs](https://gdal.org/programs/index.html) - `gdalinfo`, `gdal_translate`, `ogr2ogr`, `gdalwarp`, and more.
- [Rasterio CLI](https://rasterio.readthedocs.io/en/stable/cli.html) - `rio` commands for raster workflows.
- [rio-cogeo](https://cogeotiff.github.io/rio-cogeo/) - Create and validate COGs.
- [tippecanoe](https://github.com/felt/tippecanoe) - Build vector tiles from large GeoJSON-like inputs.
- [mapshaper](https://mapshaper.org/) - Simplify, inspect, convert, and repair vector data.
- [osmium-tool](https://osmcode.org/osmium-tool/) - OSM extract, filter, merge, and conversion workflows.
- [duckdb](https://duckdb.org/docs/stable/clients/cli/overview.html) - Local analytical SQL, including spatial extension support.
- [sqlite-utils](https://sqlite-utils.datasette.io/) - CLI and Python tools for SQLite workflows.
- [datasette](https://datasette.io/) - Publish and explore data, including spatial datasets with plugins.

## Datasets and Data Portals

- [OpenStreetMap](https://www.openstreetmap.org/) - Global community-built map data.
- [Geofabrik Downloads](https://download.geofabrik.de/) - Regional OpenStreetMap extracts.
- [Overpass Turbo](https://overpass-turbo.eu/) - Query OpenStreetMap interactively.
- [Natural Earth](https://www.naturalearthdata.com/) - Public domain small-scale cultural and physical map data.
- [GADM](https://gadm.org/) - Global administrative boundaries.
- [geoBoundaries](https://www.geoboundaries.org/) - Open administrative boundary datasets.
- [Humanitarian Data Exchange](https://data.humdata.org/) - Humanitarian and crisis-related geospatial data.
- [OpenTopography](https://opentopography.org/) - Topography and LiDAR datasets.
- [USGS EarthExplorer](https://earthexplorer.usgs.gov/) - Landsat, DEMs, aerial imagery, and other USGS datasets.
- [NASA Earthdata Search](https://search.earthdata.nasa.gov/) - NASA Earth observation data.
- [Copernicus Data Space Ecosystem](https://dataspace.copernicus.eu/) - Sentinel and Copernicus data access.
- [NASA GIBS](https://earthdata.nasa.gov/eosdis/science-system-description/eosdis-components/gibs) - Global Imagery Browse Services for rapid access to Earth observation data.
- [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/) - Cloud-hosted geospatial datasets and STAC API.
- [AWS Open Data Registry](https://registry.opendata.aws/) - Public datasets on AWS, including geospatial and climate data.
- [Google Earth Engine Data Catalog](https://developers.google.com/earth-engine/datasets) - Searchable Earth Engine dataset catalog.
- [NOAA Data Search](https://www.ncei.noaa.gov/access/search/index) - Weather, climate, ocean, and geophysical data.
- [WorldPop](https://www.worldpop.org/) - Population distribution datasets.
- [Open Buildings](https://sites.research.google/open-buildings/) - Building footprint datasets.
- [Global Human Settlement Layer](https://ghsl.jrc.ec.europa.eu/) - Built-up areas, population, and settlement layers.
- [HydroSHEDS](https://www.hydrosheds.org/) - Hydrological data and watershed products.
- [SoilGrids](https://soilgrids.org/) - Global soil property maps.

## Learning Resources

- [Geographic Data Science with Python](https://geographicdata.science/book/intro.html) - Open book on spatial data science using Python.
- [GeoPandas User Guide](https://geopandas.org/en/stable/docs/user_guide.html) - Official guide for vector GIS workflows.
- [Automating GIS Processes](https://autogis-site.readthedocs.io/) - Open course for Python GIS automation.
- [Python for Geographic Data Analysis](https://pythongis.org/) - Practical geospatial Python lessons.
- [Earth Lab Python Courses](https://www.earthdatascience.org/courses/) - Earth data science tutorials and courses.
- [NASA ARSET Trainings](https://appliedsciences.nasa.gov/join-mission/training/english/arset) - Applied remote sensing training.
- [Google Earth Engine Tutorials](https://developers.google.com/earth-engine/tutorials) - Official Earth Engine tutorials.
- [OpenGeoHub Summer School Materials](https://opengeohub.org/summer-school/) - Spatial modeling and Earth observation learning materials.
- [PySAL Notebooks](https://pysal.org/notebooks/intro) - Spatial analytics examples.
- [OSMnx Examples](https://github.com/gboeing/osmnx-examples) - Example notebooks for street network analysis.
- [Rasterio Topics](https://rasterio.readthedocs.io/en/stable/topics/index.html) - Raster workflow explanations.
- [Xarray Tutorials](https://tutorial.xarray.dev/) - Tutorials for labeled multidimensional data.
- [Dask Tutorial](https://tutorial.dask.org/) - Scalable Python workflows.
- [STAC Tutorials](https://stacspec.org/en/tutorials/) - Learn the SpatioTemporal Asset Catalog ecosystem.

## Standards and Formats

- [OGC Standards](https://www.ogc.org/standards/) - Open geospatial standards.
- [EPSG Registry](https://epsg.org/) - Coordinate reference system definitions.
- [GeoPackage](https://www.geopackage.org/) - SQLite-based geospatial exchange format.
- [GeoJSON](https://geojson.org/) - JSON encoding for geographic features.
- [GeoParquet](https://geoparquet.org/) - Parquet-based vector geospatial format.
- [FlatGeobuf](https://flatgeobuf.org/) - Streaming-friendly binary vector format.
- [Cloud Optimized GeoTIFF](https://www.cogeo.org/) - Cloud-native raster format pattern.
- [NetCDF](https://www.unidata.ucar.edu/software/netcdf/) - Multidimensional scientific data format.
- [CF Conventions](https://cfconventions.org/) - Climate and forecast metadata conventions.
- [Zarr](https://zarr.dev/) - Chunked N-dimensional array storage.
- [STAC](https://stacspec.org/) - Catalog standard for spatiotemporal assets.
- [PMTiles](https://docs.protomaps.com/pmtiles/) - Single-file archive format for tiled maps.
- [Mapbox Vector Tile Specification](https://github.com/mapbox/vector-tile-spec) - Vector tile encoding specification.
- [3D Tiles](https://www.ogc.org/standard/3dtiles/) - Streaming massive 3D geospatial content.
- [WMS](https://www.ogc.org/standard/wms/) - Web Map Service.
- [WFS](https://www.ogc.org/standard/wfs/) - Web Feature Service.
- [OGC API Features](https://ogcapi.ogc.org/features/) - Modern web API standard for feature data.

## Communities and News

- [FOSS4G](https://foss4g.org/) - Global Free and Open Source Software for Geospatial conference.
- [OSGeo](https://www.osgeo.org/) - Open Source Geospatial Foundation.
- [PyData](https://pydata.org/) - Scientific Python community with geospatial overlap.
- [Pangeo](https://pangeo.io/) - Community for scalable geoscience data analysis.
- [Project Pythia](https://projectpythia.org/) - Community learning resources for geoscience Python.
- [OpenStreetMap Community](https://community.openstreetmap.org/) - OSM discussions and local communities.
- [GIS Stack Exchange](https://gis.stackexchange.com/) - Q&A for GIS and geospatial development.
- [r/gis](https://www.reddit.com/r/gis/) - GIS community discussion.
- [This Week in OpenStreetMap](https://weeklyosm.eu/) - OSM news roundup.
- [MapScaping Podcast](https://mapscaping.com/podcast/) - Geospatial industry interviews and technical discussions.

## Contributing

Suggestions are welcome. Good additions should be:

- Useful for Python geospatial, mapping, GIS, Earth observation, or spatial data work.
- Actively maintained, widely used, or uniquely valuable.
- Linked to official documentation, a stable project page, or a well-maintained repository.
- Described with one concise sentence.

