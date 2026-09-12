# Air-Sea Heat Flux Analysis over the Bay of Bengal, Monsoon 2024

## Overview
This project computes and analyzes air-sea heat exchange over the Bay of
Bengal during the 2024 monsoon season (June–September), using Sensible Heat
Flux (SHF) and Latent Heat Flux (LHF) — two key measures of how the ocean
transfers heat and moisture to the atmosphere.

## Objective
- Compute SHF and LHF over the Bay of Bengal for the 2024 monsoon season using
  wind, sea surface temperature, air temperature, and humidity data
- Analyze how these fluxes vary spatially (across the Bay) and temporally
  (month-to-month and hour-to-hour) during the monsoon
- Compute the Bowen ratio (the ratio of SHF to LHF) to understand whether
  heat exchange is dominated by direct warming of the air or by evaporation
- Examine along-latitude variation of the fluxes using Hovmöller (time vs.
  longitude) plots

## Data
- **Source:** Gridded reanalysis data (NetCDF) — wind components (u10, v10),
  sea surface temperature (sst), 2m air temperature (t2m), and relative
  humidity across pressure levels
- **Time period:** June–September (JJAS) 2024 — the Indian monsoon season
- **Region:** Bay of Bengal

## Tools & Methods
- **Language:** Python
- **Key libraries:** xarray, numpy, matplotlib, cartopy, pandas
- **Method:** Calculated wind speed from wind components, derived saturation
  and actual vapor pressure from temperature and humidity, then computed SHF
  and LHF using standard bulk aerodynamic formulas. Analyzed the results as
  time series (overall and hourly mean), monthly spatial maps (June–September),
  the Bowen ratio (spatially and as a smoothed time series), and Hovmöller
  diagrams at two latitude bands (10°N and 20°N)

## Results
- Both SHF and LHF showed clear temporal variation across the monsoon months,
  with LHF (evaporative heat loss) generally the dominant flux, consistent
  with the Bay of Bengal being a major moisture source for the monsoon
- Spatial maps for June through September showed how the heat flux pattern
  shifts across the Bay as the monsoon progresses
- The Bowen ratio analysis showed the relative balance between sensible and
  latent heat loss changing over the monsoon season and across locations
- Hovmöller plots at 10°N and 20°N revealed differences in flux behavior
  between the southern and northern Bay of Bengal over time

## Skills Demonstrated
- Air-sea interaction and boundary-layer flux computation
- Working with multi-variable gridded reanalysis data (NetCDF)
- Spatial, temporal, and Hovmöller (time-longitude) analysis
- Scientific visualization using Python (cartopy, matplotlib)

## Author
Aaroksh Chauhan — M.Sc. Atmospheric and Oceanic Sciences, IIT Bhubaneswar
