5/10/24 notes - was looking at different merging options also

was working on getting us missing latitude and longitude coordinates until i had actual work to do at work last night and then ran out of time at work. im planning on revisiting getting our missing latitude and longitude coordinates for the SHD.csv 

when I wake up later I'm gonna work on that.

5/13/24 notes
Similar to Mark's suggestion, I'm thinking we should use city,state to get us missing lat, lon coordinates instead of using school name. Because like I mentioned, during one of my earlier experiments, the Geocode API can't find some schools or will give us an entirely different location.

SUCCESS! I have the code for us to pull latitude and longitude coordinates from City,State information

5/13 - 5/14 (days/nights blur together...)
NOTE: when plotting latitude and longitude w/ hvplot, you MUST place longitude FIRST and then latitude. otherwise it will not plot correctly

prototype map uploaded. fiddling around with the different sizes for our points. This is still off of only 1 DataFrame that hasn't been merged with others yet.