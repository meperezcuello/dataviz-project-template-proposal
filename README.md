# Data Visualization Project

## Data

The data I propose to visualize for my project is the The [World of Warcraft Avatar History Dataset](https://gist.github.com/meperezcuello/38533ec33abb5e0b3568fa4f91d97bb3) which is a **collection of records that detail information about player characters** that was cleaned and limited to less than 2 days of hourly data (since the dataset was limited to 5 mb). Understanding players behavior over playing time, allows the developers to examine posibles updates. futhermore, good Viz allows proper predict gaming time for any future update or server optimization and maintenance (you would not performing a maintenance, when most of your player population is online.

## Prototypes

For better overview of the data I've decided to plot two Viz: **the first one**, consist of the total number of player per hour over 12 hours of gameplay, with the objective to perform data manipulation on JS and D3.js without performing it offline (i.e. using Python lib such as Numpy or Pandas). Since, the Data do not show the total number per hour, instead each unique player id and a time it was connected, this transformation was required. **The latter Viz**, was a small prototype to visualize as much data in one plot, the idea is to create Viz that contains as much information of the dataset; this plot show the total level per race and character class.

[![image](https://raw.githubusercontent.com/meperezcuello/dataviz-project-template-proposal/master/%23numberplayerconencted.png)](https://beta.vizhub.com/meperezcuello/15362afeabb94920b4c1fd8175464829)

**Figure 1.** WOW Avatar History Under: Amount Players Connected per Hour

[![image](https://raw.githubusercontent.com/meperezcuello/dataviz-project-template-proposal/master/racevslevel.png)](https://beta.vizhub.com/meperezcuello/0eca535128ec4e0bb3c5e03866adad68)
  
**Figure 2.** WOW Avatar History (Race vs Total Level)

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:
(Note: might change later as the project develops over time).

* How many players are connected in one zone at one specifc time?
* What race or charclass of players is most popular in one zone during a specifc time?
* Top 5 for each zone of most popular races?
* Top 5 for each zone of most popular charclass?
* Concentraction of players levels in a specifc zone? (Useful to determine popular area for high levels char)

## Sketches

**First Sketch:** This sketch is a unique, since it helps visualize the entire playing time or behavior of every single player (ID) recorded on the datasets. As we can see, there are time tha no data was recorded between two points(hours), meaning that the player was disconnected. This sketch is related to the question, How many players are connected in one zone at one specific time?, since it expanded the question into more details, however this plot has its cons. Such as to many data might not viable to visualize in on single plot.

![image](https://raw.githubusercontent.com/meperezcuello/dataviz-project-template-proposal/master/PlayerID%20vs%20Time.jpeg)

**Second Sketch:** This sketch similar to the last one however instead of unique ID, the Viz explore the total number of player per zone and charclass in a animeted timeline of 24 to 48 hours (can be less or more). This plot is a bar plots, which is easier to interpret compared to other complex model we will see, which means user can easily identify the answer they are seeking. This chart answers the question, What race or charclass of players is most popular in one zone during a specifc time?, due to the it shows most of the data information such as charclass on x time.

![image](https://raw.githubusercontent.com/meperezcuello/dataviz-project-template-proposal/master/Most%20Popular%20CharClass%20per%20Zone.jpeg)


**Third Sketch:** Finally, we plot the desnity of player on the real map of WOW, i.e., total number of player per zone. This plot shows a real-time animation of how the desnity of each zone change over time, which can be useful to track content and utilities that might be useful for future updates. Also, this plot anwsers questions, Concentraction of players levels in a specifc zone?, as explained before.

![image](https://raw.githubusercontent.com/meperezcuello/dataviz-project-template-proposal/master/WOW%20Player%20Zone%20Density%20over%2048%20hours.jpeg)

## Open Questions

The only uncertainty that might occur during the development of this project is time concern to learn the libraries to design the WOW maps either in three.js, TopoJson.js or SVG or any data manipulation techniques.
