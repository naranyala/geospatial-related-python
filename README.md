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
- [Geocoding, Search, and Places](#geocoding-search-and-places)
- [Routing, Mobility, and Transport](#routing-mobility-and-transport)
- [Earth Observation and Remote Sensing](#earth-observation-and-remote-sensing)
- [Climate, Weather, Ocean, and Hydrology](#climate-weather-ocean-and-hydrology)
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
- [Numba](https://numba.pydata.org/) - JIT compilation for accelerating numerical spatial algorithms.
- [pybind11](https://pybind11.readthedocs.io/) - C++ bindings often used in performance-sensitive geospatial Python packages.

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
- [geohash2](https://github.com/dbarthe/geohash) - Geohash encoding and decoding utilities.
- [python-geohash](https://github.com/hkwi/python-geohash) - Fast geohash operations for Python.
- [pygeos](https://pygeos.readthedocs.io/) - Vectorized GEOS bindings; functionality was merged into Shapely 2.
- [geojson](https://github.com/jazzband/geojson) - Python helpers for GeoJSON objects.
- [TopoJSON](https://github.com/mattijn/topojson) - Convert and work with TopoJSON from Python.
- [geofileops](https://geofileops.readthedocs.io/) - Batch vector geoprocessing on files using GeoPandas, GDAL, and SQLite.
- [geocube](https://corteva.github.io/geocube/) - Rasterize vector data into gridded Xarray datasets.

## Raster and Gridded Data

- [Rasterio](https://rasterio.readthedocs.io/) - Raster I/O and processing.
- [rioxarray](https://corteva.github.io/rioxarray/stable/) - Rasterio-powered geospatial extension for Xarray.
- [Xarray](https://docs.xarray.dev/) - Labeled multidimensional arrays.
- [MetPy](https://unidata.github.io/MetPy/latest/) - Tools for reading, visualizing, and calculating with weather data.
- [Dask](https://docs.dask.org/) - Parallel and out-of-core array/dataframe computation.
- [Zarr](https://zarr.readthedocs.io/) - Chunked, compressed N-dimensional arrays for cloud and local storage.
- [rasterstats](https://pythonhosted.org/rasterstats/) - Zonal statistics over raster data.
- [xarray-spatial](https://xarray-spatial.org/) - Raster and terrain analytics using Xarray-compatible arrays.
- [rio-cogeo](https://cogeotiff.github.io/rio-cogeo/) - Cloud Optimized GeoTIFF creation and validation.
- [rio-tiler](https://cogeotiff.github.io/rio-tiler/) - Read raster tiles from COGs and other sources.
- [rio-mbtiles](https://github.com/mapbox/rio-mbtiles) - Export rasters to MBTiles.
- [verde](https://www.fatiando.org/verde/latest/) - Processing, gridding, and interpolation for spatial data.
- [xESMF](https://xesmf.readthedocs.io/) - Regridding for geospatial and climate datasets.
- [rio-viz](https://github.com/rasterio/rio-viz) - Visualize rasters from the command line and browser.
- [rio-color](https://github.com/mapbox/rio-color) - Color correction plugin for Rasterio.
- [rio-hist](https://github.com/mapbox/rio-hist) - Histogram matching plugin for Rasterio.
- [rio-mucho](https://github.com/mapbox/rio-mucho) - Parallel raster processing with Rasterio.
- [rio-tiler-pds](https://github.com/developmentseed/rio-tiler-pds) - Tilers for public satellite datasets.
- [rio-tiler-mosaic](https://github.com/developmentseed/rio-tiler-mosaic) - MosaicJSON support for rio-tiler.
- [large-image](https://girder.github.io/large_image/) - Tile-based access and visualization for large images, including geospatial rasters.
- [elevation](https://github.com/bopen/elevation) - Command line and Python tools for acquiring SRTM elevation data.

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
- [geoplotlib](https://github.com/andrea-cuttone/geoplotlib) - Python toolbox for interactive geographic visualizations.
- [mplleaflet](https://github.com/jwass/mplleaflet) - Export Matplotlib plots to interactive Leaflet maps.
- [ipygany](https://github.com/jupyter-widgets-contrib/ipygany) - 3D scientific visualization widgets for Jupyter.
- [geemap charting](https://geemap.org/) - Earth Engine-backed map widgets and analysis helpers.

## Spatial Analysis

- [PySAL](https://pysal.org/) - Spatial analysis ecosystem.
- [libpysal](https://pysal.org/libpysal/) - Spatial weights, example datasets, and core PySAL utilities.
- [esda](https://pysal.org/esda/) - Exploratory spatial data analysis.
- [spreg](https://pysal.org/spreg/) - Spatial regression.
- [mgwr](https://pysal.org/notebooks/model/mgwr/intro.html) - Multiscale geographically weighted regression.
- [segregation](https://pysal.org/segregation/) - Spatial segregation measures.
- [momepy](https://docs.momepy.org/) - Urban morphology analysis.
- [PyGeodesy](https://mrjean1.github.io/PyGeodesy/) - Geodetic and geodesic calculations.
- [MovingPandas](https://movingpandas.org/) - Trajectory data analysis.
- [scikit-mobility](https://scikit-mobility.github.io/scikit-mobility/) - Human mobility analysis.
- [Tobler](https://pysal.org/tobler/) - Areal interpolation and dasymetric mapping.
- [GeoStat-Framework](https://geostat-framework.readthedocs.io/) - Geostatistics, random fields, variograms, and kriging.
- [GSTools](https://geostat-framework.readthedocs.io/projects/gstools/) - Spatial random fields and geostatistical tools.
- [PyKrige](https://geostat-framework.readthedocs.io/projects/pykrige/) - Kriging interpolation.
- [scikit-gstat](https://scikit-gstat.readthedocs.io/) - Variogram analysis.
- [scipy.spatial](https://docs.scipy.org/doc/scipy/reference/spatial.html) - KD-trees, triangulation, Voronoi diagrams, and distance computations.
- [alphashape](https://alphashape.readthedocs.io/) - Alpha shape concave hull calculations.
- [pointpats](https://pysal.org/pointpats/) - Point pattern analysis.
- [spaghetti](https://pysal.org/spaghetti/) - Spatial network analysis.
- [inequality](https://pysal.org/inequality/) - Spatial inequality measures.
- [access](https://pysal.org/access/) - Spatial accessibility metrics.
- [giddy](https://pysal.org/giddy/) - Spatial dynamics and mobility analysis.
- [spopt](https://pysal.org/spopt/) - Spatial optimization models.

## OpenStreetMap and Networks

- [OSMnx](https://osmnx.readthedocs.io/) - Street networks, routing graphs, and OSM feature downloads.
- [Pyrosm](https://pyrosm.readthedocs.io/) - Read OpenStreetMap PBF files into GeoDataFrames.
- [osmium-tool](https://osmcode.org/osmium-tool/) - Command line OSM data processing.
- [pyosmium](https://docs.osmcode.org/pyosmium/latest/) - Python bindings for osmium.
- [NetworkX](https://networkx.org/) - Graph algorithms used in many network workflows.
- [Pandana](https://udst.github.io/pandana/) - Network accessibility analysis.
- [OSM2Pandas](https://github.com/iamtekson/osm2pandas) - Convert OSM data into pandas/GeoPandas-friendly tables.
- [OpenRouteService Python](https://openrouteservice-py.readthedocs.io/) - Client for routing, isochrones, and geocoding.
- [Overpass API Python Wrapper](https://github.com/mvexel/overpass-api-python-wrapper) - Query OpenStreetMap Overpass API from Python.
- [overpy](https://github.com/DinoTools/python-overpy) - Python client for Overpass API responses.
- [osm2geojson](https://github.com/aspectumapp/osm2geojson) - Convert OSM JSON/XML to GeoJSON.
- [osm2pgsql](https://osm2pgsql.org/) - Import OpenStreetMap data into PostgreSQL/PostGIS.
- [imposm](https://imposm.org/) - Import OpenStreetMap data into PostGIS.
- [openstreetmap-carto](https://github.com/gravitystorm/openstreetmap-carto) - CartoCSS style used for the standard OpenStreetMap map.

## Geocoding, Search, and Places

- [Nominatim](https://nominatim.org/) - Open-source geocoder powered by OpenStreetMap data.
- [Photon](https://photon.komoot.io/) - Open-source geocoder built for OpenStreetMap search.
- [Pelias](https://pelias.io/) - Modular open-source geocoder.
- [Addok](https://addok.readthedocs.io/) - Geocoding engine focused on address search.
- [Whoosh](https://whoosh.readthedocs.io/) - Pure-Python search library useful for lightweight place indexes.
- [Geocoder](https://geocoder.readthedocs.io/) - Unified Python client for multiple geocoding providers.
- [geopy](https://geopy.readthedocs.io/) - Python client for geocoding services and distance calculations.
- [OpenAddresses](https://openaddresses.io/) - Open address data from around the world.
- [WhosOnFirst](https://www.whosonfirst.org/) - Gazetteer and placetype hierarchy for places.
- [GeoNames](https://www.geonames.org/) - Global geographical names database.

## Routing, Mobility, and Transport

- [Valhalla](https://valhalla.github.io/valhalla/) - Open-source routing engine for cars, bikes, pedestrians, multimodal, and isochrones.
- [OSRM](https://project-osrm.org/) - High-performance OpenStreetMap routing engine.
- [GraphHopper](https://www.graphhopper.com/open-source/) - Open-source routing engine with road network and optimization tooling.
- [OpenTripPlanner](https://www.opentripplanner.org/) - Multimodal trip planning using transit schedules and street networks.
- [AequilibraE](https://www.aequilibrae.com/latest/python/index.html) - Transport modeling, traffic assignment, and accessibility in Python.
- [R5](https://github.com/conveyal/r5) - Rapid realistic routing on multimodal transport networks.
- [r5py](https://r5py.readthedocs.io/) - Python interface to R5 for travel time matrices and accessibility.
- [GTFS Kit](https://mrcagney.github.io/gtfs_kit_docs/) - Python tools for analyzing GTFS feeds.
- [Partridge](https://github.com/remix/partridge) - Fast GTFS feed parsing.
- [transitfeed](https://github.com/google/transitfeed) - Tools for working with GTFS transit data.
- [MovingPandas](https://movingpandas.org/) - Movement trajectory analytics with GeoPandas.
- [scikit-mobility](https://scikit-mobility.github.io/scikit-mobility/) - Human mobility metrics, preprocessing, and models.

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
- [landsatxplore](https://github.com/yannforget/landsatxplore) - Search and download Landsat scenes from USGS.
- [sentinelsat](https://sentinelsat.readthedocs.io/) - Search and download Sentinel satellite images.
- [eodag](https://eodag.readthedocs.io/) - Search and download Earth observation products from multiple providers.
- [sat-search](https://github.com/sat-utils/sat-search) - STAC search command line and Python client.
- [sat-stac](https://github.com/sat-utils/sat-stac) - STAC object helpers.
- [pyresample](https://pyresample.readthedocs.io/) - Resampling of geospatial image data.
- [Spectral Python](https://www.spectralpython.net/) - Hyperspectral image processing.
- [Orfeo ToolBox](https://www.orfeo-toolbox.org/) - Open-source remote sensing image processing toolkit with Python bindings.
- [SNAPista](https://snap-contrib.github.io/snapista/) - Python interface for ESA SNAP workflows.
- [pyroSAR](https://pyrosar.readthedocs.io/) - SAR metadata handling, archive management, and processing helpers.
- [MintPy](https://mintpy.readthedocs.io/) - InSAR time-series analysis.
- [ISCE2](https://github.com/isce-framework/isce2) - InSAR scientific computing environment.
- [isce3](https://github.com/isce-framework/isce3) - Modern InSAR processing framework.
- [OpenDroneMap](https://www.opendronemap.org/) - Open-source photogrammetry for drone imagery, orthomosaics, point clouds, and 3D models.

## Climate, Weather, Ocean, and Hydrology

- [Pangeo](https://pangeo.io/) - Community and software patterns for scalable geoscience analysis.
- [Project Pythia](https://projectpythia.org/) - Learning resources and cookbooks for geoscience Python.
- [Iris](https://scitools-iris.readthedocs.io/) - Analysis and visualization of meteorological and oceanographic datasets.
- [MetPy](https://unidata.github.io/MetPy/latest/) - Meteorological calculations, units, and data parsing.
- [cf_xarray](https://cf-xarray.readthedocs.io/) - CF Convention-aware Xarray operations.
- [xclim](https://xclim.readthedocs.io/) - Climate indices and indicators using Xarray.
- [climpred](https://climpred.readthedocs.io/) - Verification of weather and climate forecasts.
- [xskillscore](https://xskillscore.readthedocs.io/) - Forecast verification metrics for Xarray objects.
- [intake-esm](https://intake-esm.readthedocs.io/) - Catalogs for Earth system model data.
- [xgcm](https://xgcm.readthedocs.io/) - Grid-aware operations for finite-volume model output.
- [xhistogram](https://xhistogram.readthedocs.io/) - Fast histograms for Xarray and Dask arrays.
- [xesmf](https://xesmf.readthedocs.io/) - Universal regridding for geospatial datasets.
- [cfgrib](https://github.com/ecmwf/cfgrib) - GRIB support for Xarray.
- [Herbie](https://herbie.readthedocs.io/) - Download and open recent and archived weather model output.
- [Siphon](https://unidata.github.io/siphon/latest/) - Access remote geoscience data services from Python.
- [Py-ART](https://arm-doe.github.io/pyart/) - Weather radar data analysis.
- [wradlib](https://docs.wradlib.org/) - Weather radar processing.
- [HydroMT](https://deltares.github.io/hydromt/latest/) - Build and analyze hydrological and geospatial models.
- [PyFlwDir](https://deltares.github.io/pyflwdir/latest/) - Fast flow direction and hydrological network operations.
- [Landlab](https://landlab.readthedocs.io/) - Earth surface process modeling.
- [FloPy](https://flopy.readthedocs.io/) - Python tools for MODFLOW groundwater models.
- [PCRaster](https://pcraster.geo.uu.nl/) - Environmental modeling language and Python framework.
- [PyGMT](https://www.pygmt.org/) - Python interface to the Generic Mapping Tools.

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
- [stac-fastapi](https://stac-utils.github.io/stac-fastapi/) - Build STAC APIs with FastAPI.
- [stactools](https://stactools.readthedocs.io/) - Command line and library tools for working with STAC.
- [stac-validator](https://github.com/stac-utils/stac-validator) - Validate STAC catalogs, collections, and items.
- [cogeo-mosaic](https://developmentseed.org/cogeo-mosaic/) - Build and use mosaic indexes for Cloud Optimized GeoTIFFs.
- [cogdumper](https://github.com/developmentseed/cogdumper) - Inspect COG internals.
- [cogeo-watchbot](https://github.com/developmentseed/cogeo-watchbot) - Serverless COG processing pipelines.
- [xpublish](https://xpublish.readthedocs.io/) - Publish Xarray datasets through web APIs.
- [intake](https://intake.readthedocs.io/) - Data cataloging and loading framework.
- [intake-stac](https://github.com/intake/intake-stac) - Intake plugin for STAC catalogs.

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
- [GeoTrellis](https://geotrellis.io/) - Scala/Spark geospatial raster processing ecosystem with related Python integrations.
- [GeoPySpark](https://github.com/locationtech-labs/geopyspark) - Python bindings for GeoTrellis on Spark.
- [RasterFrames](https://rasterframes.io/) - Raster processing on Apache Spark.
- [GeoWave](https://locationtech.github.io/geowave/) - Distributed geospatial and spatiotemporal indexing.
- [MobilityDB](https://mobilitydb.com/) - Moving-object and temporal geospatial database built on PostgreSQL and PostGIS.
- [pgRouting](https://pgrouting.org/) - Routing and network analysis extension for PostgreSQL/PostGIS.
- [pg_tileserv](https://github.com/CrunchyData/pg_tileserv) - Vector tile server for PostGIS.
- [pg_featureserv](https://github.com/CrunchyData/pg_featureserv) - Lightweight OGC API Features server for PostGIS.
- [TimescaleDB](https://www.timescale.com/) - PostgreSQL extension useful for spatiotemporal time-series data with PostGIS.
- [rasdaman](https://rasdaman.org/) - Array database for multidimensional raster and coverage data.
- [TileDB](https://tiledb.com/) - Multidimensional array storage engine used for dense and sparse scientific data.
- [ClickHouse geospatial functions](https://clickhouse.com/docs/en/sql-reference/functions/geo) - Geospatial functions in the open-source columnar database.
- [Datashader](https://datashader.org/) - Large-scale rasterization and visualization for big spatial data.

## Data Engineering and Orchestration

- [Apache Airflow](https://airflow.apache.org/) - Platform to programmatically author, schedule and monitor workflows.
- [Dagster](https://dagster.io/) - Orchestration tool for data assets.
- [dbt](https://www.getdbt.com/) - Analytics engineering using SQL.
- [Prefect](https://www.prefect.io/opensource) - Python workflow orchestration for data pipelines.
- [Kedro](https://kedro.org/) - Data science pipeline framework.
- [Pooch](https://www.fatiando.org/pooch/latest/) - Data download and cache management for scientific projects.
- [intake](https://intake.readthedocs.io/) - Lightweight data cataloging and access.
- [frictionless-py](https://framework.frictionlessdata.io/) - Validate and describe tabular data packages.

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
- [MMDetection](https://mmdetection.readthedocs.io/) - Object detection framework often adapted for aerial imagery.
- [MMSegmentation](https://mmsegmentation.readthedocs.io/) - Semantic segmentation framework used in remote sensing research.
- [Detectron2](https://detectron2.readthedocs.io/) - Computer vision framework used for aerial object detection and segmentation.
- [Kornia](https://kornia.readthedocs.io/) - Differentiable computer vision library for PyTorch.
- [DINOv2](https://github.com/facebookresearch/dinov2) - Self-supervised vision models often used as feature encoders for remote sensing.
- [Prithvi](https://github.com/NASA-IMPACT/hls-foundation-os) - NASA/IBM open-source geospatial foundation model for Harmonized Landsat Sentinel-2 data.
- [Clay Foundation Model](https://github.com/Clay-foundation/model) - Open-source Earth observation foundation model.
- [Terratorch](https://github.com/IBM/terratorch) - Fine-tuning toolkit for geospatial foundation models.
- [YOLT](https://github.com/CosmiQ/yolt) - Object detection for overhead imagery.

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
- [OpenDroneMap](https://www.opendronemap.org/) - Photogrammetry toolkit for processing aerial imagery into maps and 3D assets.
- [WebODM](https://www.opendronemap.org/webodm/) - Browser-based interface for OpenDroneMap workflows.
- [OpenSfM](https://opensfm.org/) - Structure-from-motion library used in photogrammetry pipelines.
- [Entwine](https://entwine.io/) - Point cloud indexing and streaming.
- [Potree](https://potree.org/) - WebGL point cloud renderer.
- [CloudCompare](https://www.cloudcompare.org/) - Open-source 3D point cloud and mesh processing application.
- [pyntcloud](https://pyntcloud.readthedocs.io/) - 3D point cloud processing with pandas and NumPy.
- [trimesh](https://trimesh.org/) - Mesh processing and geometry operations.
- [gplately](https://gplates.github.io/gplately/) - Plate tectonic reconstruction and analysis in Python.
- [pyGPlates](https://www.gplates.org/docs/pygplates/) - Python bindings for GPlates plate tectonic reconstruction.

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
- [MapServer](https://mapserver.org/) - Mature open-source platform for publishing spatial data and maps.
- [GeoServer](https://geoserver.org/) - Open-source server for sharing geospatial data.
- [pygeoapi](https://pygeoapi.io/) - OGC API server implementation in Python.
- [GeoNode](https://geonode.org/) - Open-source geospatial content management platform.
- [MapProxy](https://mapproxy.org/) - Tile cache and proxy for WMS, WMTS, TMS, and other map services.
- [T-Rex](https://t-rex.tileserver.ch/) - Vector tile server for PostGIS.
- [TileServer GL](https://tileserver.readthedocs.io/) - Serve vector and raster tiles.
- [Tileserver-php](https://github.com/maptiler/tileserver-php) - Lightweight server for MBTiles.
- [Protomaps](https://protomaps.com/) - Open-source PMTiles tooling and web map stack.
- [OpenMapTiles](https://openmaptiles.org/) - Open-source vector tiles and map schema.
- [Maputnik](https://maputnik.github.io/) - Visual editor for MapLibre/Mapbox styles.
- [Tangram](https://tangrams.readthedocs.io/) - WebGL map renderer.

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
- [pmtiles](https://docs.protomaps.com/pmtiles/cli) - Command line tools for PMTiles archives.
- [planetiler](https://github.com/onthegomap/planetiler) - Build vector tiles from OpenStreetMap and other sources.
- [tilemaker](https://tilemaker.org/) - Make vector tiles from OpenStreetMap PBF files.
- [ogr2osm](https://github.com/pnorman/ogr2osm) - Convert OGR-supported formats to OpenStreetMap XML.
- [geojson-cli](https://github.com/mapbox/geojson-cli) - Command line tools for GeoJSON transformations.
- [geojsonhint](https://github.com/mapbox/geojsonhint) - Validate GeoJSON from the command line.
- [ndjson-cli](https://github.com/mbostock/ndjson-cli) - Useful streaming utilities for large GeoJSON/NDJSON workflows.
- [jq](https://jqlang.github.io/jq/) - JSON processor often used in geospatial data pipelines.

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
- [OpenAerialMap](https://openaerialmap.org/) - Open aerial imagery catalog.
- [OpenHistoricalMap](https://www.openhistoricalmap.org/) - Open historical map data.
- [OpenRailwayMap](https://www.openrailwaymap.org/) - Railway infrastructure map based on OpenStreetMap.
- [Daylight Map Distribution](https://daylightmap.org/) - Validated OpenStreetMap distribution.
- [Overture Maps](https://overturemaps.org/) - Open map data for places, buildings, transportation, and boundaries.
- [Source Cooperative](https://source.coop/) - Cloud-native open geospatial data exchange.
- [STAC Index](https://stacindex.org/) - Searchable index of STAC catalogs and tools.
- [Radiant MLHub](https://mlhub.earth/) - Open Earth observation training datasets.
- [SpaceNet](https://spacenet.ai/datasets/) - Open satellite imagery datasets for ML challenges.
- [xView](https://xviewdataset.org/) - Large-scale overhead imagery object detection dataset.
- [BigEarthNet](https://bigearth.net/) - Sentinel-2 benchmark archive for remote sensing ML.
- [SEN12MS](https://mediatum.ub.tum.de/1474000) - Sentinel-1/2 multisensor dataset with land-cover labels.
- [Chesapeake Bay Land Cover](https://lila.science/datasets/chesapeakelandcover) - High-resolution land cover dataset.
- [ESA WorldCover](https://esa-worldcover.org/) - Global land cover products.
- [Dynamic World](https://dynamicworld.app/) - Near-real-time global land cover probabilities.
- [Copernicus DEM](https://spacedata.copernicus.eu/collections/copernicus-digital-elevation-model) - Global digital elevation model.
- [MERIT Hydro](https://hydro.iis.u-tokyo.ac.jp/~yamadai/MERIT_Hydro/) - Global hydrography data.
- [FABDEM](https://data.bris.ac.uk/data/dataset/s5hqmjcdj8yo2ibzi9b4ew3sn) - Forest and buildings removed global DEM.
- [JRC Global Surface Water](https://global-surface-water.appspot.com/) - Global surface water occurrence and change.
- [OpenLandMap](https://openlandmap.org/) - Environmental layers and soil property maps.
- [Natural Earth Vector](https://github.com/nvkelso/natural-earth-vector) - Natural Earth vector source repository.
- [TIGER/Line Shapefiles](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html) - U.S. Census Bureau geographic boundary files.
- [US Census Cartographic Boundary Files](https://www.census.gov/geographies/mapping-files/time-series/geo/cartographic-boundary.html) - Simplified U.S. boundaries for mapping.
- [Bureau of Transportation Statistics Geospatial Data](https://geodata.bts.gov/) - U.S. transportation geospatial datasets.
- [OpenAQ](https://openaq.org/) - Open air quality data.
- [GBIF](https://www.gbif.org/) - Global biodiversity occurrence data.
- [iNaturalist Open Data](https://www.inaturalist.org/pages/developers) - Biodiversity observations and media metadata.

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
- [Pangeo Gallery](https://gallery.pangeo.io/) - Reproducible examples for scalable geoscience workflows.
- [Project Pythia Cookbooks](https://cookbooks.projectpythia.org/) - Community geoscience Python recipes.
- [The Carpentries Geospatial Lessons](https://carpentries-incubator.github.io/geospatial-python/) - Introductory geospatial Python lessons.
- [QGIS Training Manual](https://docs.qgis.org/latest/en/docs/training_manual/) - Practical open-source GIS concepts and workflows.
- [PostGIS Introduction](https://postgis.net/workshops/postgis-intro/) - Hands-on spatial SQL tutorial.
- [MapLibre Examples](https://maplibre.org/maplibre-gl-js/docs/examples/) - Web map examples using MapLibre GL JS.
- [OpenStreetMap Wiki](https://wiki.openstreetmap.org/) - Documentation for OSM tagging, data model, and tooling.
- [NASA Earthdata Tutorials](https://www.earthdata.nasa.gov/learn) - Earthdata learning resources and recipes.

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
- [OGC API Tiles](https://ogcapi.ogc.org/tiles/) - Standard for tiled geospatial resources.
- [OGC API Coverages](https://ogcapi.ogc.org/coverages/) - Standard for coverage data APIs.
- [WMTS](https://www.ogc.org/standard/wmts/) - Web Map Tile Service.
- [TMS](https://wiki.osgeo.org/wiki/Tile_Map_Service_Specification) - Tile Map Service specification.
- [MBTiles](https://github.com/mapbox/mbtiles-spec) - SQLite-based tile archive format.
- [LAS](https://www.asprs.org/divisions-committees/lidar-division/laser-las-file-format-exchange-activities) - ASPRS LiDAR point cloud exchange format.
- [EPT](https://entwine.io/entwine-point-tile.html) - Entwine Point Tile format for streaming point clouds.
- [GTFS](https://gtfs.org/) - General Transit Feed Specification.
- [GTFS Realtime](https://gtfs.org/documentation/realtime/reference/) - Realtime transit updates.
- [OpenAPI](https://www.openapis.org/) - API description standard used by many OGC API implementations.

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
- [CUGOS](https://cugos.org/) - Cascadia Users of Geospatial Open Source.
- [GeoHipster](https://geohipster.com/) - Interviews and commentary from the geospatial community.
- [OpenCage Geomob](https://thegeomob.com/) - Geospatial meetups, talks, and podcast.
- [OpenStreetMap US](https://openstreetmap.us/) - U.S. OpenStreetMap community and events.
- [HOT OpenStreetMap Team](https://www.hotosm.org/) - Humanitarian mapping community.
- [Spatial Data Science Conference](https://spatial-data-science-conference.com/) - Spatial analytics and data science conference.

## Contributing

Suggestions are welcome. Good additions should be:

- Useful for Python geospatial, mapping, GIS, Earth observation, or spatial data work.
- Actively maintained, widely used, or uniquely valuable.
- Linked to official documentation, a stable project page, or a well-maintained repository.
- Described with one concise sentence.
