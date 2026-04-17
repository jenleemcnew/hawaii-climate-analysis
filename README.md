# Hawaii Climate Analysis

## Overview
A climate analysis and Flask API project exploring weather data from Hawaii 
weather stations. Uses SQLAlchemy ORM to query a SQLite database of historical 
precipitation and temperature observations, with results visualized in Pandas 
and served via a REST API.

---

## Part 1 — Climate Analysis

### Precipitation Analysis
- Identified the most recent date in the dataset
- Queried the previous 12 months of precipitation data
- Loaded results into a Pandas DataFrame and plotted rainfall over time
- Generated summary statistics for precipitation data

### Station Analysis
- Calculated total number of weather stations in the dataset
- Identified the most active station by observation count
- Queried lowest, highest, and average temperatures for the most active station
- Plotted 12 months of temperature observations as a histogram

---

## Part 2 — Climate Flask API

| Route | Description |
|-------|-------------|
| `/` | Homepage listing all available routes |
| `/api/v1.0/precipitation` | Last 12 months of precipitation data as JSON |
| `/api/v1.0/stations` | List of all weather stations as JSON |
| `/api/v1.0/tobs` | Last 12 months of temperature observations for most active station |
| `/api/v1.0/<start>` | Min, avg, and max temps from start date to end of dataset |
| `/api/v1.0/<start>/<end>` | Min, avg, and max temps for a specified date range |

---

## Tech Stack
- Python (SQLAlchemy, Pandas, Matplotlib, Flask)
- SQLite
- Jupyter Notebook

---

## Repository Contents
| File | Description |
|------|-------------|
| `climate_starter.ipynb` | Climate analysis notebook |
| `app.py` | Flask API application |
| `hawaii.sqlite` | SQLite climate database |
