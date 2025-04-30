# <Repository Title>
<Instructions: copy and paste this template into your project README file (found in the parent folder of the repository). Fill in relevant information as requested.>

<General notes: add as much information as is relevant for your repository. Some overarching guidelines are provided, but feel free to expand on these guidelines.>
<More resources found here: https://www.dataone.org/all-best-practices>
<Delete the text inside the brackets when formatting your file.>

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
- Raw: Contains the USGS data after it had been retrieved from USGS using the 'dataRetrieval' package.
- Processed: Contains the mean daily discharge and mean monthly discharge for each gage, as well as the combined files for each gage.

The Project_Files folder contains 6 .rmd files.
- Data_Analysis: File where data was analyzed with a time series analysis.
- Data_Exploration: File where the data was explored through plots and tables.
- Data_Processing: File where the data was cleaned.
- Final_Project_Report: The final report for the course project.


<describe the folders contained in the repository, including what type of files they contain>

<describe the formats of files for the various purposes contained in the repository>

<describe your file naming conventions>

## Metadata

<For each data file in the repository, describe the data contained in each column. Include the column name, a description of the information, the class of data, and any units associated with the data. Create a list or table for each data file.> 

## Scripts and code

<list any software scripts/code contained in the repository and a description of their purpose.>
