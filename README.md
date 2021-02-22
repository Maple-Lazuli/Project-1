# Using demographic and crime data to decide where to live

## Motivation
This is my first dive into a solo analysis using linear regression and US census data. My hope is to answer the following questions:
1. Can I predict crimes of rape, arson, vehicle theft, larceny, burglary, robbery, and aggravated assault using demographic data?
2. Can I determine which demographic fields are the most useful for such predictions? 
3. Can I apply the models to predict crime rates for some of the cities I'm considering moving to?

## Resources Utilized
### Python Libraries
The following python libraries were utilized:
1. numpy
2. pandas
3. matplotlib
4. sklearn
5. seaborn

### Library Installation
Execute the following code either in an interactive python shell or
from a python script and the packages should be installed:
```Python
import subprocess
import sys
packageList = ['numpy','pandas','matplotlib','sklearn','seaborn']
for package in packageList:
    subprocess.check_call([sys.executable, "-m", "pip", "install", package]) 
```

## Repository Contents
The itemized list below details the files found in the repository
1. Census_demographics_by_County.csv  - Dataset containing demographic data by county in the united states
2. US_States.csv - Dataset containing a mapping of US states to a numeric designation.
3. crime_data_w_population_and_crime_rate.csv - Dataset containing crime data by county in the united states
4. 'Where To Live.ipynb' - A jupyter notebook containing code and analysis to the questions posed in the motivation.

## Results

The model worked very well for predictions on crime for counties, but did not work very well for predictions on cities. 

## Sources and Acknowledgements
### Code and Methodology
The methodology around the use of linear regression and reviewing the weights came from what I learned in the Udacity Data Science nanodegree program 
(https://www.udacity.com/course/data-scientist-nanodegree--nd025)

### Dataset Sources

1. Census_demographics_by_County.csv - from Arcgis at: https://hub.arcgis.com/datasets/6afda9afb9f94e27adf39d36e119eb29_2

2. US_States.csv - from Arcgis at: https://hub.arcgis.com/datasets/utah::us-states

3. crime_data_w_population_and_crime_rate.csv - from Kaggle at: https://www.kaggle.com/mikejohnsonjr/united-states-crime-rates-by-county
