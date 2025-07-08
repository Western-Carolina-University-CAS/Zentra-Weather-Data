# Zentra-Weather-Data

Public CSV archive of historical and daily-updated Zentra environmental sensor readings.

---

## Available Datasets

| Location             | Device SN | Location                  |
| -------------------- | --------- | ------------------------- |
| Gribble Gap Riparian | z6-12561  | 35.3035251, -83.2058057   |
| Gribble Gap Upland   | z6-12514  | 35.3073691, -83.209171    |
| Cullowhee Creek      | z6-12516  | 35.3104179, -83.1874281   |
| Long Branch Upland   | z6-12512  | 35.3044209, -83.208245    |
| Long Branch Riparian | z6-12513  | 35.3047241, -83.2018152   |

---
## File Format

Each CSV is in **wide format**, one row per timestamp and one column per sensor measurement.  


---

## Update Schedule

These files are re-generated and committed **once daily**, pulling the latest data from the Zentra API.

---

## How to Download

1. **Download via link:**
  [zentra_weather_data.zip](https://github.com/Western-Carolina-University-CAS/Zentra-Weather-Data/raw/refs/heads/main/data/zentra_weather_data.zip)

2. **Clone** this repo:  
   ```bash
   git clone https://github.com/Western-Carolina-University-CAS/Zentra-Weather-Data.git
   ```
3. **Download via curl**

   ```bash
   curl -O https://github.com/Western-Carolina-University-CAS/Zentra-Weather-Data/raw/refs/heads/main/data/zentra_weather_data.zip
   ```

4. **Download via wget**

   ```bash
   wget https://github.com/Western-Carolina-University-CAS/Zentra-Weather-Data/raw/refs/heads/main/data/zentra_weather_data.zip
   ```
---

## Sample Data

Below is a sample of the wide-format CSV data:

| timestamp_utc | datetime                 | mrid | Air Temperature ( °F) (ATM-410005328) | Atmospheric Pressure ( kPa) (ATM-410005328) | Battery Percent (%) (nan) | Battery Voltage ( mV) (nan) | EC ( mS/cm) (1702903091) | Gust Speed ( mph) (ATM-410005328) | Leaf Wetness ( min) (nan) | Leaf Wetness (high) ( min) (nan) | Lightning Activity (nan) (ATM-410005328) | Lightning Distance ( km) (ATM-410005328) | Logger Temperature ( °F) (1618462184) | Matric Potential ( kPa) (T21G20002522) | Max Precip Rate ( mm/h) (ATM-410005328) | Precipitation ( mm) (ATM-410005328) | RH Sensor Temp ( °F) (ATM-410005328) | Reference Pressure ( kPa) (1618462184) | Relative Humidity (%) (ATM-410005328) | Saturation Extract EC ( mS/cm) (T12-00053631) | Sensor Metadata (nan) (1702903091) | Soil Temperature ( °F) (T12-00053631) | Soil Temperature ( °F) (T21G20002522) | Solar Radiation ( W/m²) (ATM-410005328) | VPD ( kPa) (ATM-410005328) | Water Content ( m³/m³) (T12-00053631) | Water Level ( in) (1702903091) | Water Temperature ( °F) (1702903091) | Wetness Level (nan) (nan) | Wind Direction (°) (ATM-410005328) | Wind Speed ( mph) (ATM-410005328) | X-axis Level (°) (ATM-410005328) | Y-axis Level (°) (ATM-410005328) |
|---------------|--------------------------|------|--------------------------------------|--------------------------------------------|--------------------------|----------------------------|-------------------------|----------------------------------|-------------------------|-------------------------------|------------------------------------------|-------------------------------------|------------------------------------|-------------------------------------|---------------------------------------|------------------------------|-----------------------------|------------------------------|-------------------------------------|----------------------------------------------|-------------------------------|-------------------------------|-------------------------------|--------------------------------------|----------------------|-----------------------------|-----------------------------|-------------------------------|-------------------------|------------------------------------|--------------------------|---------------------------|---------------------------|
| 1625680800    | 2021-07-07 14:00:00-04:00 | 1    | 70.4                                 | 92.65                                     | 89.0                     | 7709.0                     |                           | 0.83                            | 0.0                     | 0.0                          | 0.0                                     | 0.0                                | 71.8                               | -18100.7                        | 0.0                                  | 0                            | 71.1                        | 92.5                        | 92.2                                | 0.05                                         |                           | 65.5                          | 65.8                          | 57.0                                 | 0.2                  | 0.367                      |                           |                           | 446.0                   | 212.0                             | 0.49                      | -0.9                      | -0.2                      |
| 1625681700    | 2021-07-07 14:15:00-04:00 | 2    | 71.0                                 | 92.63                                     | 88.0                     | 7707.0                     |                           | 0.78                            | 0.0                     | 0.0                          | 0.0                                     | 0.0                                | 71.7                               | -12058.6                        | 0.0                                  | 0                            | 71.2                        | 92.49                       | 92.0                                | 0.05                                         |                           | 65.3                          | 65.6                          | 43.1                                 | 0.21                 | 0.367                      |                           |                           | 446.0                   | 269.0                             | 0.38                      | -1.0                      | -0.2                      |
| 1625682600    | 2021-07-07 14:30:00-04:00 | 3    | 71.3                                 | 92.6                                      | 88.0                     | 7706.0                     |                           | 1.3                             | 0.0                     | 0.0                          | 0.0                                     | 0.0                                | 71.8                               | -7171.3                         | 0.0                                  | 0                            | 71.6                        | 92.46                       | 90.9                                | 0.05                                         |                           | 65.1                          | 65.4                          | 37.9                                 | 0.24                 | 0.367                      |                           |                           | 446.0                   | 238.0                             | 0.76                      | -0.9                      | -0.2                      |


---

### Column Naming Convention

All measurement columns use the format:

- **Measurement Name**: The type of measurement (e.g., Air Temperature)  
- **Unit**: The reporting units (e.g., °F, kPa, mm)  
- **Device SN**: The serial number of the sensor that produced the measurement (e.g., ATM-410005328)  

For example, `Air Temperature (°F) (ATM-410005328)` represents the air temperature in Fahrenheit, measured by sensor serial `ATM-410005328`.`
