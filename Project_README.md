# Group 1 - Project 1

The city of Newark, NJ has compiled a list of multiple abandoned and vacant buildings.  From this list, our goal was to find a correlation between this list and the factors that may have contributed to the number of abandoned properties. The overall data on city statistics of housing demographics, crime, education, and poverty were obtained and evaluated.



# Part 1 - Newark Overall Housing

The notebook for this segment appears under the "01_Newark Overall Housing Data" folder, named "HousingDataAnalysis.ipynb".

Abandoned House Data http://data.ci.newark.nj.us/dataset/abandoned-properties/resource/796e2a01-d459-4574-9a48-23805fe0c3e0
 



# Part 2 - Newark Abandoned Housing

The notebook for this segment appears under the "02_Abandoned Housing" folder, named "2_Newark_abandoned_data.ipynb".

For this part you will need the following to run this notebook:
1) Your Google.com API key as g_key in the file named api_keys.py (saved to the "02_Abandoned Housing" folder)
2) Install geocoder from the Terminal (see https://pypi.org/project/geocoder)

The processes below yield outputs that have been saved in a folder located "02_Abandoned Housing/output".

The Newark_abandoned_data notebook calls a JSON file from the City of Newark website obtaining a list of abandoned properties by address. (http://data.ci.newark.nj.us/dataset/abandoned-properties/resource/796e2a01-d459-4574-9a48-23805fe0c3e0)

Building DataFrames from this source allows us to utilize various functions to manipulate the data for analytical purposes.

KEY FACTORS

Translate DataFrame headers (keys) for context of the data
Build out full address including city, state, and zip code (used for next steps)

NOTE: the zip code collection for loop will run for approx. 5 minsutes before completing the process
----------------------------------------------------------------------------------------------------------------------
Add longitude and latitudes to the addresses for use in mapping (using geocoders)

Additional actions
Extract the summaries by year, zip code and other useful criteria for abandoned properties on the list.  
These summaries should be compatible with other data (poverty, crime, etc.)

Map the abandoned addresses on a map of Newark, NJ
Pie plot showing the relative percentages of abandoned property by zip code



# Part 3 - Poverty Rate Data Analysis

For Poverty Analysis portion of the group project:
-Jupyter Notebook: Newark Poverty Rate.ipynb under folder names 05_Crime_Data_Study
    -Open after Abandoned Housing analysis portion (Tim Weir’s branch of the project)
    -Pulls data from newark_abandoned_data.csv (in data folder) and combines with: 
        -US Census American Community Survey 5-Year Data (for 2019)
            - https://api.census.gov/data/2019/acs/acs5?get=NAME,group(B01001)&for=us:1
        -Google gmaps API
-Census Exception message after running Data Retrieval cell, still allows other cells to run
-Cleaned data set used for heatmap:
    -newark_poverty_population.csv in output folder
        -analysis takeaways at the end of the notebook done with Excel
-Poverty "Heat" Map:
    -newark_poverty_map.png in output folder 




# Part 4 - Education

The notebooks for this segment appears under the "04_Education" folder, named "CollegeINFO.ipynb" and "HighSchoolINFO.ipynb".




# Part 5 - Crime Data Study

The notebooks for this segment appears under the "05_Crime_Data_Study" folder, named "5a_combined_Crime_UCR_2018_2019_2020.ipynb" and "5b_crime_data_Newark.ipynb".
