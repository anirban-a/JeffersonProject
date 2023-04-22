# Jefferson Project

## Analysis of `Phycocyanin` concentration as a key to detect Algal bloom in Lake George.

<hr>

### Hypothesis and exploration questions
1. Phycocyanin level variation in different seasons.
2. Phycocyanin level variation across 2017 - 2019.
3. How is solar radiation impacting the concentration?
4. What kind of relations exist between phycocyanin concentration and water acidity/alkalinity.

### Executing the scripts to generate data for analysis

1. Execute [solar_radiation_data_wrangle.ipynb](EDA%2Fdata.wrangling%2Fsolar_radiation_data_wrangle.ipynb)
   and [vp_data_wrangle.ipynb](EDA%2Fdata.wrangling%2Fvp_data_wrangle.ipynb) in any order.
2. Execute [integrate_vp_solar_rad.ipynb](EDA%2Fdata.wrangling%2Fintegrate_vp_solar_rad.ipynb). This will merge the cleaned data from above 2 steps into a new `csv` file.
3. Execute [nutrients_data_wrangle.ipynb](EDA%2Fdata.wrangling%2Fnutrients_data_wrangle.ipynb). This will merge nutrients data into the `csv` file formed in the above step.
4. Execute [NASA_power_data_wrange.ipynb](EDA%2Fdata.wrangling%2FNASA_power_data_wrange.ipynb). This will merge NASA data into the `csv` file formed in the above steps.

### Executing the scripts to generate data for forecasting
1. Execute [vp_data_wrangle_fc.ipynb](EDA%2Fdata.forecast.wrangling%2Fvp_data_wrangle_fc.ipynb)
2. Execute [nutrient_data_wrangle_fc.ipynb](EDA%2Fdata.forecast.wrangling%2Fnutrient_data_wrangle_fc.ipynb)
3. Execute [prepare_forecast_input.ipynb](EDA%2Fdata.forecast.wrangling%2Fprepare_forecast_input.ipynb)

## Data dictionary

| Variable          | Definition                                                    |
|-------------------|---------------------------------------------------------------|
| TP                | total phosphorus                                              |
| TSP               | total soluble phosphorus                                      |
| SRP               | soluble reactive phosphorus                                   |
| TN                | total nitrogen                                                |
| NO3               | nitrate                                                       |
| NH4               | ammonium                                                      |
| PP                | particulate phosphorus                                        |
| PRECTOTCORR       | Precipitation Corrected (mm/day)                              |
| ALLSKY_SFC_SW_DWN | All Sky Surface Shortwave Downward Irradiance (kW-hr/m^2/day) |
| ALLSKY_SFC_LW_DWN | All Sky Surface Longwave Downward Irradiance (kW-hr/m^2/day)  |
