# Data Literacy Fatal Accidents Analysis
This project aims to evalute irresponsible driving based on fatal car accidents in the US.
## File structure:
Code expects data in the following file structure:

```
**root**
-- **data** all Data files should be placed here
---- **Google_daten(US).csv** Full Dataset could be found [here](https://storage.googleapis.com/covid19-open-data/v2/main.csv) _note: Only import US data (start_line=14096993,nrows=2368485)_
---- **people.csv** Full Dataset can be found [here](https://www2.census.gov/programs-surveys/popest/datasets/2020-2021/counties/totals/co-est2021-alldata.csv)
---- **FARS2021NationalCSV** Full Dataset can be found [here](https://www.nhtsa.gov/file-downloads?p=nhtsa/downloads/FARS/2020/National/)
------ **accident.csv**
------ **...**
------ **weather.csv**
---- **County shape data** Used for Geoplot. Dataset can be found [here](https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html)
------ **...**
---- **States shape data** Used for Geoplot. Dataset can be found [here](https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html)
------ **...**
--**doc**
---- **project_report**
------ **...** all Latex files
-- **plots** interesting graphs are saved in this folder
---- **...**
-- **Car accident analysis.ipynb** programm file for analysis
```
## How to run "Car accident analysis.ipynb":
requirements:
```
pandas >= 2.0.0
numpy >= 1.26.0
matplotlib >= 3.7.0
matplotlib_venn
os
datetime
tueplots
sklearn
seaborn >= 0.13.0
geopandas
contextily
logging
```
Download all data files and place them in the data folder. 

## Data Explanation:
### FARS2021National
Includes all data on accidents, involved vehicles and persons.
key:[Case,Vehicle_num,Person_num]
### Google_daten(US).csv
Original designed to analyse Covid. This includes detailed information about population, demographic, area and weather for all states and counties in the USA.
key:[Day,State/County]
### shape data
used for plotting (includes the shape of counties/states)
