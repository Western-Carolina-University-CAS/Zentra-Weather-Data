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
3. **Download a single CSV file with curl**

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


<sub>**Columns shown**: This is a partial preview for readability; actual CSVs have additional measurements and columns (including all units in headers).</sub>
