# Prevalence of School Shootings in the US

Team Members: Adriel, Jayce, William, Vivian, Christian, Levi \
Repo owner: Levi

## Project Description/Outline:
 School shootings are a highly controversial topic in the US, our group is interested in looking at trends of the shootings and understanding patterns that may arise or have been prevalent over the years. 

## Research Questions to Answer:
1. Which regions or states have experienced the highest and lowest incidences from 1999 - 2023?
2. How have the yearly and monthly trends of school shootings fluctuated over the past few decades, and what seasonal patterns are evident?
3. What are the patterns among different incidents in terms of location (urban vs. rural, region), time of day (morning vs. afternoon), and weapon type?
4. Are certain types of schools, such as elementary, high schools, or private institutions, more vulnerable to school shootings?
5. What traits are common among perpetrators (Age, gender, race, mental health history, planned vs. not planned, etc.)?
6. What risk factors or warning signs, such as mental health issues or behavioral problems, the situation of the incident are often identified before an incident?


## Datasets to be used:
- Kaggle School Shootings (J. ARVIDSSON) : https://www.kaggle.com/datasets/joebeachcapital/school-shootings?select=school-shootings-data.csv

- Kaggle School Shootings (S. KAPADNIS): https://www.kaggle.com/datasets/sujaykapadnis/school-shooting-data?resource=download&select=dataset.csv

- CHDS School Shooting Safety Compendium: https://www.chds.us/sssc/data-map/

- (Link to the website we pulled the excel file from; independent reporters:)
https://www.motherjones.com/politics/2012/12/mass-shootings-mother-jones-full-data/

##
# Final Analysis:
Based on our data visualization plots, we can observe that:
- From the year range of 1999-2023, the states with the highest incidences were California and Texas while the lowest was New Hampshire and North Dakota
- In the past 25 years, the number of school shootings has been slightly increasing
- The type of school that have the highest amount of incidents are High Schools
- Shooters are most likely to start an incident during the mornings and afternoons and during the Fall and Winter
- Shooters are predominately male and a lot of them do not have a history of bullying or domestic violence
- The most common choice of weapon among shooters is a pistol 
- Most shooting incidents are not planned
- The mean of shooters age is 16 with an outlier of 72 years old


##
# Project Details:
## Roles
Every team member collaborated equally throughout the journey of the project. Although the roles are listed below, members collaborated and assisted others interchangeably

Adriel: Cleaning data/Visual graphics\
Jayce: Finding missing Longitude/Latitude data\
William: Final analysis/Presentation prep\
Vivian: Cleaning data/readme\
Christian: Visual analysis

## Cleaning Data Workflow:
1. Go through each csv and include desired columns into a dataframe
2. Format Date in a specific format (take year from the "Date" column in Kaggle_2 csv)
3. Proper casing columns and necessary rows
4. Filling NA's with "Unknown"
5. Making sure School type columns appear in a similar format for all dataframes ("Middle" will turn into "Middle School")
6. Making sure all states are in the same format\
a. This was done by installing "us" and importing it.\
b. To take abbreviations of states for the shd_df and converting them into the full name of the states, create and utilize a function
7. Exporting cleaned dataframes to a new csv file
8. Merging "right" on columns that will display the most and relevant data 
9. Discussing with the team which _x or _y columns to include and exclude
10. Dropping undesired columns and duplicates
11. Exporting the final clean dataframe into a new csv file for later use and manipulation

## Filling Missing Latitudes and Longitudes:
1. Load csv files, drop Latitude and Longitude to make way for new coordinates
2. Define a function utilizing the geoapify url to pull coordinates appropiately 
3. Create a loop to begin the search and load new found coordinates into designated columns
4. Output updated csv's for later use for geomap

## Displaying our Findings Visually:
To observe annual and monthly trends of school shootings:
- We created a bar chart that reveals overall shooting trends by month and year
- Bar chart for seasonal incidents, and quarter incidents

To observe regions and states affected by shooting incidents:
- We created a geomap of the US displaying the prevalence
- We created a bar chart to display the top five schools

To analyze patterns based on school type, time of day, and location:
- We created bar charts to visualize incident patterns by school type (elementary, high school) and time of day (morning vs. afternoon).
- We created a pie chart to show the distribution of weapon types used.

To analyze perpetrator demographics:
- We created pie charts to represent the gender distribution and common weapon usage
- Bar chart was created to display the count of ages amongst shooters


## Final Analysis folder tour:
In the "Resources" folder, the orginal csv files utilized are stored:
- Kaggle1DS.csv
- Kaggle2DS.csv
- SHD.csv

Master jupyter notebook:
- Final_Notebook.ipynb

Outputs such as CSV files and PNG files found in "Outputs" folder


