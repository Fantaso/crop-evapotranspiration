# crop-evapotranspiration

This model is design by FAO and its use for calculating the amount of water that is lost due to evaporation or absorbed by the plant due to transpiration during the cultivation cycle.

this water lost calculated through this method helps farmers to irrigation schedules and quantity that must be replaced for the crop during a period of time considering factors such as weather data, crop height and grass height.

The output of this script gives mm depth of water which is usually the number used to irrigate the fields.

## STEP # 1
### VARIABLES AND CONSTANTS
---
Add variables and constants
* aerodynamic_resistance
* surface_resistance
* average_atmospheric_pressure
* psychrometric_constant
* air_temp_mean
* actual_vapour_pressure
* actual_vapour_pressure_rh


# STEP # 2
## WEATHER ANALYSIS
---
* **ALTITUDE** abovve sea level
* **LATITUDE & LONGITUDE** location
* **TEMPERATURE** average, daily min and max temperature using mean air temperature instead of maximum and minimum air temperatures yields a lower saturation vapour pressure es, and hence a lower vapour pressure difference (es - ea), and a lower reference evapotranspiration estimate.
* **HUMIDITYY** with psychomretric or dewpoint temp or min and max relative humidity
* **WIND SPEED** at 2 meter above soil, if at different height a modification most be calculated


## STEP # 3
### SUN ANALYSIS
---
* **EXTRATERRESTRIAL RADIATION**  radiation that reacvh atmosphere [MJ / m2 * day]
* _daily or shorter periods measurements_


## STEP # 4
### SOIL ANALYSIS
---
* **SOIL HEAT FLUX (G)**

## STEP # 5
### WIND ANALYSIS
---
**WIND PROFILE RELATIONSHIP**
* Wind speeds measured at different heights above the soil surface are different. Surface friction tends to slow down wind passing over it. Wind speed is slowest at the surface and increases with height.
* For this reason anemometers are placed at a chosen standard height, i.e.,10 m in meteorology and 2 or 3 m in agrometeorology. For the calculation of evapotranspiration, wind speed measured at 2m above the surface is required. To adjust wind speed data obtained from insruments placed atelevations other than the standard height of 2 m, a logarithmic wind speed profile may be used for measurements above a short grassed surface

1. u2 = wind speed at 2 m above ground surface [m / s]
2. uz = measured wind speed at z m above ground surface [m * s]
3. z = height of measurement above ground surface [m]
* The corresponding multipliers or conversion factors are given in Annex 2 (Table 2.9) and are plotted in Figure 16.

## STEP # FINAL
### EVAPOTRANSPIRATION CROP REFERENCE ANALYSIS
