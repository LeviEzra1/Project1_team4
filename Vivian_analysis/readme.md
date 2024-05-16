# Work Flow Process

Log 5/15/24:\
After doing the biggest data clean up for the final merged df, I realized after looking at everyone's work that I was supposed to include a README file... So I will include it now!

## Initital intentions:
When doing our own independent merges, I've realized that I would be needing to do way more work in terms of cleaning to properly have 3 fairly large csv's to merge smoothly. With this in mind, I made it my main goal to do as much cleaning to make the data as uniform as possible.

## Role
I took on the role of cleaning up and merging the csv's.

## Tasks:
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

## My analysis folder tour:
In my folder, I have the orginal csv files from our sources:
- Kaggle1DS copy.csv
- Kaggle2DS copy.csv
- SHD copy.csv

My original/drafted jupyter notebook:
- Vivi_Draft.ipynb

Cleaned csv files exported from my notebook:
- clean 1 .csv
- clean 2 .csv
- clean 3 .csv
- Final_Data .csv

After discussing with the group, and having them select my notebook for the master notebook for our project, we further cleaned my drafted notebook and ended up with:
- Final_Data.ipynb\
(This was later added onto the Final Analysis folder)

This readme file:
- readme.md