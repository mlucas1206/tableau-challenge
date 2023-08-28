# CitiBike Tableau Visualization July 2023
Tableau Link: https://public.tableau.com/app/profile/miggy.lacson/viz/CitiBikeAssignment_16928476354280/StartMapsandEndMaps#1

## Dataset Used
This is my CitiBike project done for my bootcamp at Rutgers. The data I am using from the source is 3 July's from 2021 to 2023. 


## Visualization focus
Our instructions were to find phenomena that we can focus on and to visualize. We were going to look for something unusual in the data. The ones I chose to pursue were
1) Market share of the bike type being used; and
2) The share of the uses based on member types

We were also required to make a map with a zipcode overlay.


## Limitations and Clean up Processes
1) I only used 1 month from 3 different years since my machine can only process 3-4 months worth of data. To add, 2020 and previous years have a slightly different data columns than 2021 onwards. I decided to only use the 3 latest years to have consistency.


2) I placed the files into pandas in python and firstly removed all the records with at least a null field. I concatenated them into one dataframe and selected only the data I need. This will lessen the stress on the machine as I remove unnecessary data. 


3) I had to replace the coordinates column since the coordinates per address are not consistent thus making them unable to visualize the map properly. What I did is I averaged the coordinates per address and used that to represent their location. 


## Visualization Tabs
### Maps
I made maps with the zipcode overlay and the heatmap for which stations are being used more. If you toggle between the years, you can see that some stations dont appear in them. Can the data really show that the stations weren't used or does not all data make it to the system? One thing we can make out from the heat map is that the bikes are mostly used in Manhattan, where a big chunk of that is in midtown to downtown area. This could be because of all the offices and other establishments that can be found here compared to Upper Manhattan. Check the second and third portions of this story board.


### Membership
First set of visualizations are related to the division of the uses if it was by a member or a casual user. We can see from the 1st graph that the amount of uses by members gets a bigger share on each year, possibly due to the increase of active users becoming members. The next 2 graphs shows percentage and actual numbers of each member type through the years. We can see that the casual uses are stagnant under 900,000 in the past two years while member uses shot up by 824,369 or a whopping 39.43% increase.


### Bike Type
The second set of data I wanted to look at was the bike types given in the data. If you look at the Type Use Count visual, we can see that the docked bike is very immaterial. Which raises the question what these are or why they were counted. To avoid this type the other 2 graphs were made filtering out docked bikes. The line graph below shows that the classic bike has similar trends evry year and peaks at 5 or 6 pm. With the upper left graph, we can raise a question why electric bikes are being used less and less. Are they being phased out? Are they always broken? We have to be able to understand the data they have before making any proper analysis.