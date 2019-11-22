# ProjectOneTeamJay
### Team Members:
### Alexandra Oricchio, Jessica Kim, Youssef Mroue

## Project Description/Outline
Understanding gun violence in the U.S. between 2013 and 2018.

## Research Questions to Answer
Which states have the top percentage of incidents per capita?

How does the average number of people injured per incident vary per state?

What was the most frequent incident type per state? by year?
  
## Data Sets to be Used
* [Gun Violence Data] (https://www.kaggle.com/jameslko/gun-violence-data)
* [GMaps API's](developers.google.com/apis-explorer)
* [Government](census.gov/data.html)
* [Wrapper for the United States Census Bureau's API] (https://github.com/datamade/census)

## Parameters and Limitations of our Data Sets
* Gun Violence Data:
  * Includes data for gun violence incidents in the United States that occurred between 2013 and 2018.
  * Includes data for all 50 states and includes District of Columbia as its own state
  * What qualifies as a gun violence incidet? A gun violence incidents includes, but is not limited to, armed robberies, pistol whipping, suicide...
* Census Data:
  * Includes the 5 year average population per state (2011 - 2016)
  
 ## Important to Note
 * Per capita calculations are based on per 10,000
 * In regards to incident type, one gun violence incident can be counted as multiple incident types. For example, a single incident involving drug use and suicide would be counted twice as two different incident types.
 
 ## Project Structure
How our project repository is structured:
* __Data folder:__
  * __raw_data folder:__ this folder contains our raw data. We added this folder to our gitignore as the raw data set was too large to upload to github. 
  * __notebooks folder:__
    * __Census_Extract.ipynb:__ Jupyter Notebook using the python wrapper for the United States Census Bureau's API to pull the 5 year average population per state and exporting data into a csv file. 
    * __Cleanup1.ipynb:__ Jupyter notebook used to clean and filter our raw data into a new dataframe and exporting cleaned data into a csv file. 
   * __clean_data folder:__
      * __census_data.csv:__ csv output from "Census_Extract.ipynb" notebook. This csv file includes the 5 year average population per state.
      * __clean_data.csv:__ csv output from "Cleanup1.ipynb" notebook. This csv file is our cleaned dataset and includes the population data pulled from US Census. 
* __Notebooks folder:__ We split our data exploration into three main topics and worked in individual notebooks to conduct further analysis on these three topics. 
  * __allie.ipynb:__ Allie’s notebook explores the outcome of gun violence incidents in the United States. More specifically, Allie explores the top ten states based on the total number killed and total number injured by a gun related event. Allie’s notebook also explores these results on a per capita basis to examine how population effects these results.  
  * __Jess.ipynb:__ Jess’s notebook explores the frequency of gun violence incidents in the United States. Jess conducted an analysis on the top ten states based on total number of gun violence incidents and the top ten states based on total number of gun violence incidents per capita. 
  * __youssef.ipynb:__ Youssef’s notebook focuses on the top types of gun violence in the United States. In order to analyze this data, Youssef first conducted a text analysis of our raw data. Youssef’s analysis resulted in a clean and functional data set depicting the types of gun violence incidents occurring in the United States. Youssef then took this data set and analyzed the top five types of gun violence incidents and created gmap visuals to show where these incidents appear to be occurring most throughout the United States. 
  * __output folder:__ This folder contains png files for any visualiztions created in the notebooks above. 
 * __Reports folder:__
  * __Final_analysis.ipynb__
  * __ProjectJay.ppt__
  * __ProjectJay_GunViolence.docx__
  
