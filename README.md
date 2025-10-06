# GCM Precipitation Data Processing for Historical Runs and SSP Scenarios

This project processes **CMIP6** and **CMIP5** precipitation data for both **historical model runs** and **SSP scenarios**. The scripts extract, convert, and calculate time series data at specific latitudes and longitudes, generate average precipitation values, and save the processed data in **Excel** and **text files**.

---

## Features

- **Extract precipitation data** (`pr` variable) from CMIP6/CMIP5 **.nc** files.
- **Convert precipitation units** from m/s to **mm/day**.
- **Filter data** for the required historical period or SSP4.5 scenario.
- **Calculate time series** for specific latitude and longitude coordinates.
- **Save processed data** to Excel files and text files.
- **Calculate average precipitation** across coordinates for each model run.

---

## Directory Structure

- `scripts/`: Contains Python scripts for processing precipitation data.
  - `process_precipitation_data.py`: Processes CMIP6/CMIP5 data for the **SSP4.5** scenario.
  - `process_historical_run.py`: Processes **historical model run** data from CMIP6/CMIP5 models.
  
- `data/`: Placeholder directory for your input NetCDF data files (not part of the repository).
  
- `output/`: The directory where the processed output data (Excel and text files) will be stored.

- `coordinate_timeseries.xlsx`: Excel file summarizing time series data for each coordinate.
  
- `coordinate_timeseries_txt/`: Directory containing individual text files with the average time series data for each station.

---

## How to Use

### Prerequisites

Ensure you have **Python 3.x** installed along with the required libraries:

```bash
pip install xarray pandas numpy

