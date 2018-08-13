# NOAA_US_Inclement_Weather_Analysis
- U.S. National Oceanic and Atmospheric Administration’s storm analysis
- Scientific: Climate

- Exploratory data analysis was conducted in R using U.S. National Oceanic and Atmospheric Administration (NOAA) weather data "Storm Data" data set via National Weather Service to answer the question, what is the highest ranking weather event for economic and public health impact? 


Processing Instructions:
- R script file and pdf file are included.
- To improve reproducibility of the data analysis, an R-Markdown file is included. 
- Use R Studio or other application to read R script and R-Markdown file.

Steps to Transformation:
- NOAA data were downloaded from "https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2" and loaded into R as csv file with nonrelevant variables dropped to improve import speed and analysis.
- The INJURIES and FATALITIES variables were combined into new column that is sum of fatalities and injuries; to make it easier to graph the total of fatalities and injuries..
- The associated EVTYPE was changed to all upper case to faciliate accurate grouping.
- Any zero sum values were removed from the data set as they are not needed for analysis.
- Exploratory analysis was conducted of the misspelled words in the EVTYPE variable for injuries and fatalities analysis.
- The weather event type variable (EVTYPE) was cleaned to correct obvious errors in spelling.
- The data set was grouped by EVTYPE and plotted.
- Unit value designators from the PROPDMGEXP and CROPDMGEXP variables were used to index the data set.
- A list was created to hold the unit value designators to search on and their associated base 10 value to multiply by for the found PROPDMG and CROPDMG values; these values were computed and assigned to the data set.
- Additionally PROPDMG and CROPDMG were combined into a new column that is sum of damage for each this was done to make it easier to
graph total of property and crops damages.
- The data set was grouped by EVTYPE, formatted for easier display in the visualization, and plotted.
- Visualizations were created for economic and public health impact results.
- The data shows the top 2 weather events for public health impact include: Tornado and Thunderstorm Wind, for economic
impact include: Flood and Hurricane/Typhoon.
