# Climate Data Analysis & Fire Weather Index Modelling

A series of Python notebooks exploring large-scale geospatial climate datasets, with a focus on computing the Canadian Fire Weather Index (FWI) for New Zealand using real meteorological station data.

Data sourced from the [NZ Modelling Data Consortium](https://www.envlib.org) via MetService's 20-year numerical weather dataset, accessed through the [Tethys](https://tethysts.readthedocs.io) Python library.

---

## Notebooks

### `fire_weather_index.ipynb`
Calculates the Canadian Fire Weather Index (FWI) for New Zealand locations using real FENZ weather station data. The FWI is a globally recognised metric for wildfire danger, computed from four atmospheric variables: temperature, relative humidity, wind speed, and precipitation. Includes NZ-specific latitude/longitude calibration and validation against NIWA fire weather benchmarks.

### `large_scale_climate_data.ipynb`
Demonstrates efficient handling of out-of-memory climate datasets in the hundreds of GBs to low TBs using Xarray and Dask. Covers lazy loading, chunking strategies, parallel computation, and performance optimisation for multi-file NetCDF datasets.

### `advanced_climate_analytics.ipynb`
Applies advanced analytical techniques to multi-dimensional climate data including spatial masking, temporal resampling, and groupby operations. Includes analysis of wind speed distributions filtered by temperature quantiles and computation of hourly composite averages.

### `climate_data_visualisation.ipynb`
Introduces working with NetCDF meteorological data using Xarray, covering multi-dimensional indexing, time series analysis, and spatial map generation. Uses Cartopy and Salem for projection-aware visualisation of NZ climate variables including relative humidity and wind speed.

---

## Stack

- **Python** — Xarray, Dask, NumPy, Matplotlib, Cartopy, Salem, Tethys
- **Data formats** — NetCDF (.nc)
- **Domain** — Climate science, fire weather modelling, geospatial analysis

---

## Background

Completed as part of postgraduate geospatial climate data science coursework at the University of Canterbury. The fire weather index work connects directly to applied climate risk modelling in a professional context.
