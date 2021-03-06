# Streaming Weather Data

This folder was created by a team of University of Washington Professional and Continuing Education night school students for a final project, for class Big Data 230B Emerging Technologies in Big Data 8/23/2017.

## Overview
The main components of the project are:
- A set of python scripts that use Apache Kafka and Web API's to gather weather and traffic data from Washington State Dept of Transportation (WSDOT) and Yahoo Query Language (YQL), and save to disk as JSON files.
- A Jupyter Notebook that aggregates the JSON files into data frames, and does some mapping and graphing.

| Folder    |Description |
|----------:|:-----------|
|APIs       | Sample json files from various weather & traffic API's.  Also contains csv with API calling syntax.|
|sample_code| Ignore this.  It was used in early development, then abandoned. |
|prototypes | Jupyter Notebooks which open multiple json files, combine them into data frames, then do mapping and visualization.|

|File of Interest | Description |
|----------------:|:------------|
| APIs/API_index.csv | Table of Web API's, inluding url syntax and links to documentation. |
| APIs/\*.json       | Sample Web API outputs. |
| streaming/UW_PCE_BIGDATA_230B.ipynb | Currently the best/clearest Jupyter Notebook. |
| streaming/<other ipynb files> | Draft notebooks, low quality, ignore them. |
| Open_Weather/\*.py | Kafka scripts that call openweathermap.org, resulting json has issues. |
| wsdot_weather/\*.py | Kafka scripts designed to call WSDOT and Yahoo Web API's. |

_Cool-looking tables, huh?  I learned how to do it from [adam-p's markdown cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)_

## Running the Python Kafka Scripts
[TODO] Describe the Bitnami, etc.

## Alternatives to Kafka
In theory, you could have a python script that simply runs on one machine, making web API calls and saving results to json. The use of Kafka was a class project requirement, that may or may not fit your particular use case.  

## Using the Jupyter Notebook
[TODO] Describe Conda, etc.

## Future Work
- Add isntructions for setting up Bitnami Kafka server & scripts.
- Add instructions for setting up the conda environment for Jupyter.
- Create a sandbox repo, and move a bunch of files there.
- Finalize comprehensive data frames, export to csv, upload to data.world.
  - Assemble a data dictionary for data.world.
