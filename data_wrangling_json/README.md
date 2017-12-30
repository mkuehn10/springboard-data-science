# Data Wrangling JSON Mini-Project

[Jupyter Notebook File](sliderule_dsi_json_exercise.ipynb)

## Summary
JSON data from the World Bank Project was used to examine the top 10 countires with the most projects and the top 10 major project themes.  There were several missing values for the major project themes, so steps were taken to fill in the missing values with known values from other projects (each theme is associated with a code; the codes were used to fill in the missing themes).  Through an iterative process, three methods were used to fill in the missing values:
* Manually create a dictionary that mapped the projects codes to the project themes
* Group the table by project theme and use an aggregate mean on the code column to map the codes to the themes
* Ignore the rows with missing project themes, drop duplicate rows, and use the remaining distinct rows to map the codes to the themes

## Packages Used
1) [pandas](https://pandas.pydata.org/pandas-docs/stable/)
2) [json](https://docs.python.org/3.6/library/json.html)

## Techniques Used
1) json_normalize (pandas.io.json) -- parse JSON in to tables for analysis
2) DataFrame.value_counts() -- find the top values in columns
3) DataFrame.copy() -- create a fresh copy of a DataFrame for further analysis and testing
4) zip() -- combine two lists in to a dictionary
5) DataFrame.loc and DataFrame.iloc -- filtering DataFrames by values
6) Lambda functions and DataFrame.apply() -- use a throwaway function to map values from one column to another column in a DataFrame
7) DataFrame.groupby() -- create a summary of values in a DataFrame
8) DataFrame.drop_duplicates() -- drop all duplicate rows in a DataFrame
