# Data Literacy Fatal Accidents Analysis
This analysis aims to evalute irresponsible driving in fatal accidents in the US.
## Project structure:
Code expects data in the following file structure:

**root**
-- **Daten** all Data files should be placed here
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
-- **Graphen** interesting graphs are saved in this folder
---- **...**
-- **Car accident analysis.ipynb** programm file for analysis

## How to run "Car accident analysis.ipynb":
needed librarys:
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