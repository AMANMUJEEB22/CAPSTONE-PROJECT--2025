# **Analyzing and Visualizing UNESCO Education Statistics**
The UNESCO Institute for Statistics (UIS) is the authoritative source for globally comparable data on education, science, culture, and communication. As UNESCO’s official statistical agency and custodian of Sustainable Development Goal 4 (Quality Education), UIS provides critical data to guide policies and investments that shape the future of education worldwide.This project utilizes the UIS dataset to carry out thorough data cleaning, preprocessing, and visualization. The focus is on extracting meaningful insights and trends in education statistics, particularly regarding Information and Communication Technology (ICT) graduates across various countries and years.By removing irrelevant metadata and handling missing or duplicate data, the project refines the raw dataset into a clear, analyzable form. Renaming columns and organizing data prepares it for effective visualization and further analysis.
# Data Cleaning and Visualization of UNESCO Education Data
Step 1: Dataset Loading
We began by importing the UNESCO UIS dataset (CSV format) into a Pandas DataFrame using Python. This step reads the raw data into memory so it can be processed and analyzed.
Step 2: Data Cleaning – Removing Unnecessary Columns
The original dataset contained many metadata columns that were not useful for analysis (e.g., STRUCTURE, FREQ, UNIT_TYPE, etc.). These were dropped to simplify the dataset and improve focus.
Step 3: Checking for Missing and Duplicate Values
To ensure data quality, we checked for:
Null (missing) values using isnull().sum()
Duplicate rows using duplicated().sum()
These checks help ensure the integrity of the dataset before visualization.
Step 4: Renaming Columns for Clarity
Several column names were long or unclear. We renamed key columns for readability and easier analysis. For example, REF_AREA_LABEL was renamed to Country, and OBS_VALUE to Value.
Step 5: Data Visualization
Using matplotlib and seaborn, we visualized trends in ICT-related education statistics. For example, we plotted the total number of ICT graduates by year to identify growth patterns and country-level trends.
