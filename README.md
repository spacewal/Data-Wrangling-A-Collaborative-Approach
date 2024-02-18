# Data-Wrangling-A-Collaborative-Approach

# London Bus Incident Analysis

## Overview
This repository contains a data wrangling and exploratory data analysis (EDA) project on a dataset of incidents involving London buses. The dataset includes information about incidents, such as the date, route, operator, location, type of incident, victim category, and weather conditions at the time of the incident.

## Dataset
The dataset, `London_Bus_Weather_Lambda.csv`, consists of over 10,000 rows and 24 columns. It was sourced from [add source here] and includes data from [start year] to [end year].

## Data Wrangling Steps
1. **Dataset Acquisition and Loading:** The dataset was loaded into a pandas DataFrame for analysis.
2. **Structural Investigation:** The structure of the dataset was examined, including data types and unique values.
3. **Quality Investigation:** The dataset was cleaned by removing duplicates, renaming and dropping columns, treating datetime columns, and handling missing values.
4. **Data Integration:** A secondary dataset containing additional information about bus routes was merged with the primary dataset.
5. **Data Binning:** The `mean_temp` column was binned into categories based on temperature ranges.
6. **Lambda Function Application:** A lambda function was used to create a new column based on the `mean_temp` column.
7. **Feature Engineering:** A new feature, `day_of_week`, was added to the dataset to indicate the day of the week for each incident.

## Exploratory Data Analysis
Key insights from the EDA include:
1. The majority of incidents occurred on weekdays, with Friday having the highest number of incidents.
2. The most common victim category was 'Passenger'.
3. Incidents were more frequent in colder temperatures.
4. The 'Onboard Injuries' incident event type was the most common.
5. There was a noticeable increase in incidents during the winter season.

Visualizations supporting these insights can be found in the accompanying Jupyter Notebook.

## Files
- `London_Bus_Weather_Lambda.csv`: Original dataset.
- `London_Bus_Weather_Cleaned.csv`: Cleaned dataset.
- `London_Bus_Weather_Merged.csv`: Merged dataset with additional bus route information.
- `London_Bus_Weather_Binned.csv`: Dataset with binned temperature data.
- `London_Bus_Weather_with_DayOfWeek.csv`: Dataset with added `day_of_week` feature.
- `Data_Wrangling_and_EDA.ipynb`: Jupyter Notebook containing the data wrangling and EDA process.

## Tools Used
- Python
- pandas
- NumPy
- Matplotlib
- seaborn

## Conclusion
This project provided valuable insights into the patterns and trends of incidents involving London buses. The data wrangling process helped in preparing the dataset for analysis, while the exploratory data analysis uncovered key trends that can be useful for improving bus safety and operations.
