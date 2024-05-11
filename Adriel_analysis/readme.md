I am currently working on identifying the columns to keep for a final school shooting data frame. I will split the information to columns I have kept, and also tracking columns that have been droppped. We don't have to keep all the columns I decide to keep, just working on eliminating unneccesary columns. This is currently being worked from my final_data_mergeß

Columns being kept: 'LONCOD', 'LATCOD', 'year_x', 'school', 'city_x', 'state_x', 'address', 'urbanrural', 'race', 'killed_x', 'injured_x', 'date_x', 'type', 'time_x', 'uid', 'district_name', 'school_year', 'day_of_week', 'school_type', 'casualties', 'shooting_type', 'age_shooter1', 'gender_shooter1', 'race_ethnicity_shooter1', 'shooter_relationship1', 'shooter_deceased1', 'deceased_notes1', 'resource_officer', 'weapon', 'weapon_source', 'county', 'Date', 'Quarter', 'City', 'Location', 'During_School', 'Time_Period', 'First_Shot', 'Bullied',
       'Domestic_Violence', 'Gang_Related', 'Preplanned'


Columns being dropped: 'CDCODE', 'victims', 'NCESSCH', 'nces_school_id', 'nces_district_id', 'date_y', 'year_y','time_y', 'city_y', 'state_y', 'enrollment', 'killed_y', 'injured_y', 'age_shooter2', 'gender_shooter2', 'race_ethnicity_shooter2', 'shooter_relationship2', 'shooter_deceased2', 'deceased_notes2', 'lat', 'long', 'staffing', 'low_grade', 'high_grade', 'lunch', 'state_fips', 'county_fips', 'ulocale', 'Incident_ID', 'State', 'School_Level'


Discussion: 
Let's discuss these, not sure what they are representing. I understand that it is race but maybe this is race distribution of students at school? Not sure: 'white', 'black', 'hispanic', 'asian', 'american_indian_alaska_native','hawaiian_native_pacific_islander', 'two_or_more'

We also have two lat & long (lat, long & LONCOD, LATCOD)

Getting different values for the same ID on 'Date', 'date_x' & City	city_x (going to keep them both for now so we can review them)