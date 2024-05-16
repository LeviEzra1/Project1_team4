5/10/24 notes - was looking at different merging options also

was working on getting us missing latitude and longitude coordinates until i had actual work to do at work last night and then ran out of time at work. im planning on revisiting getting our missing latitude and longitude coordinates for the SHD.csv 

when I wake up later I'm gonna work on that.

5/13/24 notes
Similar to Mark's suggestion, I'm thinking we should use city,state to get us missing lat, lon coordinates instead of using school name. Because like I mentioned, during one of my earlier experiments, the Geocode API can't find some schools or will give us an entirely different location.

SUCCESS! I have the code for us to pull latitude and longitude coordinates from City,State information

5/13 - 5/14 (days/nights blur together...)
NOTE: when plotting latitude and longitude w/ hvplot, you MUST place longitude FIRST and then latitude. otherwise it will not plot correctly

prototype map uploaded. fiddling around with the different sizes for our points. This is still off of only 1 DataFrame that hasn't been merged with others yet.

adjusting the "scale" universally adjusts the scaling of the points on the map
points "size" is currently set to number of victims (not necessarily deaths) from each of the school shootings
Although the death of a child ultimately weighs more, I think "victim count" is a more important statistic to keep track of; in an ideal world, no children would get shot while in school or even when they're not in school


We initially used "School Name" to update/populate missing "Latitude" and "Longitude" data however the Geoapify API at times would give far off coordinates based off of school name. (For one of the schools, I was given coordinates for a location in Brazil.) Our instructor suggested to get missing coordinates utilizing "City" and "State" instead; so we did and it worked beautifully. 

The "Latitude" and "Longitude" coordinates were then used to plot school shootings on an image map of the United States using the number of victims (people that were shot) as the size of the plots. Initially "Years" of the school shootings were populated when hovering over the plots. Then "City" and "School" information were added to glean more information. "Dates" of the school shootings replaced "Years" in the case that multiple school shootings occured within the same vicinity and year. NOTE: when using hvplots, "Longitude" coordinates must be given before "Latitude" coordinates since hvplots plots based off x,y coordinates and not the traditional Latitude, Longitude.

IDEAS FOR ANALYSIS:
-frequency of shootings at the same school (pie chart)