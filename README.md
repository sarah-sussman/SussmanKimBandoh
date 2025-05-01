# <SussmanKimBandoh>

## Summary
The SussmanKimBandoh repository is the final course project repository for the class ENV 872. The respository contains files for data processing, exploration, and analysis. We processed discharge data from 10 USGS stream gages before (Sept. 27,  2023 - March 27, 2024) and after (Sept. 27, 2024 - March 27, 2025) Hurricane Helene made landfall in Western NC. Our main research question is did discharge increase in the French Broad and Swannanoa Rivers after Hurricane Helene? If so, is an increase in discharge long-term, or is just in the days after the hurricane (Sept 27, 2024)? We address these research questions through calculating the mean daily and mean monthly discharge for each time period at each USGS gage location.

## Investigators
Sarah Sussman, MEM student, sarah.sussman@duke.edu
Akosua Bandoh, MEM student,akosua.bandoh@duke.edu
Yeeun Kim, MEM student, yeeun.kim@duke.edu

## Keywords
Hurricane Helene
USGS
Discharge
Time series

## Database Information

Discharge data from each gage was retrieved from the USGS using the 'dataRetrival' package (created by USGS). This data was then cleaned to only include and rename relevant columns: date, discharge (cfs), USGS gage ID number, name of gage, and time period (before or after the hurricane). USGS discharge data for all time periods was combined after pulling so that each gage station had a discharge dataset with relevant dates for mean daily and mean monthly discharge. USGS data was initially accessed on April 7, 2025.

## Folder structure, file formats, and naming conventions 

The project has two folders: Data and Project_Files

The Data folder contains two folders: Raw and Processed
- Raw: Contains the USGS data after it had been retrieved from USGS using the 'dataRetrieval' package. Includes csv titled "gage_locations" that has each gage and it's latitude and longitude.
- Processed: Contains the mean daily discharge and mean monthly discharge for each gage, as well as the combined files for each gage.

The Project_Files folder contains 6 .rmd files.
- Data_Analysis: File where data was analyzed with a time series analysis.
- Data_Exploration: File where the data was explored through plots and tables.
- Data_Processing: File where the data was cleaned.
- Final_Project_Report: The final report for the course project.

File naming conventions
river_city_variable_timeperiod

ex: FBR_Marshall_discharge_before - this file is for the USGS gage in the French Broad River in Marshall, NC. The data is for discharge and the time period is before the hurricane (Sept 27, 2023 - March 27, 2024).

## Metadata
For raw USGS discharge data:
- agency_cd : agency that collected the data
- site_no: gage id number
- dateTime: Day and time of day observation took place
- X_00060_00000: discharge in cfs
- X_00060_00000_cd: indicates the status of the observation, if it has been reviewed or not
- tz_cd: Timezone the date and time column is in

For processed USGS discharge data
- date: date of observation
- mean_daily_discharge_cfs: the mean daily discharge in cfs of that date
- mean_monthly_discharge_cfs: the mean monthly discharge of the month
- month: month the mean monthly discharge is referring to
- time_period: the before (2023-2024) or after (2024-2025) period
- name: name of gage
- ID_number: Unique USGS gae ID number
- monthly_df: Sorted monthly discharge dataset by year and month
- monthly_ts: Time series object of monthly discharge values
- monthly_stl: STL decomposition result of the monthly discharge time series
- tau_results: Kendall’s Tau trend statistics for each site and time period
- gage_list: a list of daily discharge dataframes by site with date, discharge, and time period
- combined_data: a merged dataframe of all sites’ daily discharge data with site labels included
	
## Scripts and code
N/A
