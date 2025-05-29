# los-angeles-crimes
An in-depth analysis of Los Angeles crime data from 2020 onwards, focusing on trends, patterns, and geographical distributions using Python for data cleaning, EDA, and visualization.

# Los Angeles Crime Data Analysis (2020-Present)

## Project Description
This project focuses on exploring and analyzing incident-level crime data from the City of Los Angeles, covering incidents from 2020 to the present. The aim is to uncover patterns, trends, and insights into crime occurrences across different dimensions such as time, location, and crime type. This analysis demonstrates skills in data cleaning, exploratory data analysis (EDA), and data visualization using Python.

## Problem Statement & Goals
The primary goals of this analysis are to:
* Identify the most common types of crimes reported in Los Angeles.
* Analyze crime trends over time (e.g., monthly, quarterly, yearly patterns).
* Investigate the geographical distribution of crimes to identify high-incidence areas.
* Explore relationships between crime incidents and other available attributes (e.g., victim age, sex, descent, premise description).
* Provide data-driven insights that could potentially inform community safety initiatives or resource allocation.

## Data Source
The dataset used in this project is the "Los Angeles Crime Data from 2020" provided by the Los Angeles Police Department (LAPD) via [data.gov](https://catalog.data.gov/dataset/crime-data-from-2020-to-present).

**Important Data Notes:**
* It's important to note that the crime data for 2024 and 2025 within the dataset is incomplete due to the adoption of a new Records Management System for reporting crimes and arrests by the Los Angeles Police Department in 2024. As observed in an initial time trend analysis, records for 2024 show a significant drop-off towards the latter half of the year, and 2025 only contains minimal entries. To ensure accuracy and avoid misinterpreting trends based on partial data, this project will filter the dataset to include crime incidents up to and including December 31, 2023. All analyses and findings presented are therefore based on the complete data up to the end of 2023.
* The data is transcribed from original paper crime reports and may contain some inaccuracies.
* Some location fields with missing data are noted as `(0°, 0°)`. These will require careful handling during analysis.
* Address fields are provided only to the nearest hundred block to maintain privacy.

## Technologies Used
* **Python**
* **Pandas:** For data manipulation and analysis.
* **NumPy:** For numerical operations.
* **Matplotlib:** For basic plotting and visualization.
* **Seaborn:** For enhanced statistical data visualization.
* **(Potentially others as needed):** e.g., Plotly for interactive visualizations, SciPy for statistical tests.

### Key Findings and Insights

This data analysis project investigates Los Angeles crime data from 2020 to December 31, 2023, employing statistical methods to identify and analyze prevalent crime types and their trends over time.

**Most Prevalent Crime Types:**
An examination of crime descriptions revealed the most common offenses reported in Los Angeles during the period of analysis:
* The data indicates a strong prevalence of **property-related crimes**. **"VEHICLE - STOLEN"** remains the most frequent, accounting for $\approx 10.68\%$ of all reported crimes. This is followed by **"BATTERY - SIMPLE ASSAULT,"** **"THEFT OF IDENTITY,"** and **"BURGLARY FROM VEHICLE."**
* While property crimes dominate the top ranks, the significant presence of various **assault types** highlights areas of concern beyond just property loss. These include **"BATTERY - SIMPLE ASSAULT,"** **"ASSAULT WITH DEADLY WEAPON, AGGRAVATED ASSAULT,"** and **"INTIMATE PARTNER - SIMPLE ASSAULT."**

### Crime Trends Over Time

**Crime Trends Over Time (2020-2023):**
Analyzing monthly crime trends for each year provides a visual understanding of shifts in reported incidents:

![Monthly Crime Trends in Los Angeles (2020-2023)](Monthly_Crime_Trends_LA.png)

* **Overall Increase followed by a Slight Decline:** The graph clearly illustrates that crime counts in **2022 (green line)** and **2023 (yellow line)** are consistently higher across most months compared to **2020 (black line)** and **2021 (blue line)**. This indicates a general upward trend in reported crimes from the earlier years, peaking in 2022, followed by a slight moderation in 2023.
* **Limited Consistent Monthly Seasonality:** While minor fluctuations are visible, the plot does not reveal a strong, repeatable seasonal pattern across all years (e.g., a distinct, consistent peak or trough month). This suggests that while subtle influences might be present, they aren't the primary drivers of overall crime volume in Los Angeles during this period.
* **Year-Specific Observations:**
    * **2020 (Black Line):** Represents the lowest crime reporting year in the dataset, providing a baseline.
    * **2021 (Blue Line):** Shows an increase from 2020, but generally stays below the levels of the subsequent two years.
    * **2022 (Green Line):** Stands out as the year with the highest overall monthly crime counts, indicating a peak in reported incidents during this period.
    * **2023 (Yellow Line):** While still high, this line generally runs slightly below the 2022 peak, suggesting a modest decrease or leveling off in crime reporting.

## Google Colab Notebook
[Link to Live Colab Notebook](https://github.com/vonlanot/los-angeles-crimes/blob/main/LA_Crime_Notebook.ipynb)

## How to Explore
1.  Click on the "Link to Live Colab Notebook" above.
2.  The notebook will open directly in Google Colab.
3.  You can view the code, outputs, and explanations. To run the code yourself, you can select "File" > "Save a copy in Drive" or "Save a copy in GitHub" to create your own editable version.
