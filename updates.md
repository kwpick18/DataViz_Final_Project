## March 21

Downloaded the NHL all_teams.csv file and read the file into R. Trying to narrow down the data set in order to find out what i want to work with. 

## March 23 Beginning of class

Sifted through the data to make a plan of where to go from here as well as got my data in a place where I can begin to manipulate it for the project. I chose to start small with the Pittsburgh Penguins data set and work out from there. The goal is to look at different variables available in the data and see if we find any interesting correlations, comparisons, or just anything that pops out. I will begin by categorizing the data by the situation on the ice (5on5, 5on4, etc.) 

## March 23 end of class

Continued to get my data set smaller and smaller so I can work on one particular area. Began making my first portion of the shiny app which will look at percentage of low danger, medium danger, and high danger goals for pittsburgh against each team. 

## March 28th Beginning of class

Over the weekend, I began working on the first part of my app using the low, medium, and high danger variables. As I got about an hour in and began trying to run my data that I had, I realized the variables weren't what I thought they were. Long story short, I switched my approach and began using shot attempts, shots on goal, and goals for to try to find a correlation between number of goals and shots on the power play. I'm starting small and working from there. 

## March 28th End of class

During class, I was able to troubleshoot some things I had going wrong with the first part of my app. I got my scatterplot to be reactive to what I wanted to show (goals for compared to proportion of shots getting through to the net) and began to plan the next part of my project. Next, I'd like to offer a shiny app where the user can decide what situation to look at (even strength, powerplay, PK) using radio buttons to see the trends in that data as well. 

## March 30th Beginning of Class

I was playing with my first app for some time trying to clean it up and make it look nicer. I learned how to add a title to it which was easy but I couldn't do a facet_wrap function to my scatterplot output like I would like to do. I also kind of figured out my hypothesis for what I want this project to examine. "More shots = More goals?"

## March 30th End of Class 

I made some progress in my understanding as well as in the app itself. I finally was able to facet my graphs but still not in the format that I want. I made headway on creating a reactive table below the visualization to make understanding the data easier for the viewer. I may even add panels to the app to make it less messy. 

## April 4th Beginning of Class

I updated my original parameters for the shiny app to include all situations of play for the Pittsburgh Penguins from the 2017 season instead of only using the powerplay and changed my hypothesis as well to "more shots = more goals". I made some good progress by faceting the graphs how I wanted, by situation, and beginning to make my table. The table is tricky but I almost have it sorted. 

## April 4th End of Class 

I cleaned up my tabular data in my initial shiny app by selecting only columns that I'm interested in. I spent most of the time in this class researching how to create multiple tabs and am still trouble shooting. I hope to make multiple different times looking at different statistics to answer multiple questions. 

## April 6th Beginning of Class

I figured out how to create a second tab and began working on what to put in that tab. I tried a similar thing to my first tab but I didn't like that they were almost the same thing. I'm now trying to manipulate the data so I can look at the correlation between icetime for a team on the Powerplay and total powerplay goals over the course of all seasons recorded in my data set. 

## April 6th End of Class

I manipulated the data enough for my icetime/goals/season for each team app to be able to work with it. I still have to input the set into the shiny app code but being able to have the data in a place where it makes sense is a good start. I also realized that my PP ice time wasn't per player but instead it was input as seconds of icetime. That changes things in the way the data will be presented. I will work over the weekend on completing the second tab of my app. 

## April 11th (off day) 

I changed my approach on my second panel of the slide to make it easier to read and vizualize. I ran into some trouble when trying to manipulate the data enough to have it make sense in a visualization and be helpful by i think it looks good. I changed the color scales on my bar chart but doesn't seem to be affecting the color. Ill have to figure that out for wednesday. 


## April 13th (no class) 

I've been attempting for a while now to add another reactive table to my second panel but am getting mixed up with some of my previous naming of data sets I want to use. I thought I had it correct but it still doesn't seem to be working. I will continue to attempt to make it work over the weekend with success hopefully. 

<<<<<<< HEAD

## April 18th Beginning of Class

Over the weekend, I did a complete overhaul of my second panel. I realized that it wasn't visualizing what I had hoped for and really didnt serve much of a purpose. I spent most of my time figuring out how I could get number of goals on the Y axis (which was easy) with both Icetime per season on the powerplay and the season variable both on the x-axis. I still have some work to do cleaning it up but I think the visualization will be much more clear now. I also added the table i was trying to add. 

## April 18th End of class

During class, I manipulated by ice_time_table data set to get rid of totals and began to change the names of a few variables that were not matching where i needed them to match. I also put my bar graph in descending order but still haven't gotten to making my table in descending order on my second panel. That will be first on the list for between today and wednesday. My if-else statement should fix the problem of different names for the same team. Also will be completed by Wednesday. 

## April 20th Beginning of class

Probaby doesn't look like I did much because I didn't make any progress. I labored over how to use ifelse statements for about an hour and a half before giving up and moving on to trying to arrange my tables in descending order for another 1 or so. It seems like I've tried everything by now but I guess I just don't understand the syntax and how to put it into a shiny app. 

## April 20th End Of class

I made some really good progress this class. I was going about changing my variable names all wrong. Instead of ifelse statements, I used string_replace which did the trick right away. I then had to alter my data set so that there were no duplicates which could skew the data. I finally have the second panel tidied up to where I want it to be. My plan is to add a 3rd panel that is something we haven't done in class so I can get more credit for my project and hopefully have something interesting to report! 

## April 25th Beginning of Class

Over the weekend, I did a lot of research on cool things to add to my app to make it better and more fun for the user. I added a theme adjuster to my project where the user can make it whatever color or theme they would like. I tried adding a spinning wheel when it loads new visualizations but haven't got that to work yet. I also started on making my 3rd panel which will be a "curiousity" slide for the user to do pretty much whatever they want with. 

## April 25th End of Class

I got my 3rd panel to work where the user will be able to input what they want to see and search the entire data set for what they are interested in. I will only include variables that make sense to someone who doesn't know anything about the data set such as goals for, goals against, etc. I will add radio buttons so they can choose what category and another drop down menu for the season they wish to look into. Once I get that buttoned up, the app will be in a good place! 

## April 27th Beginning of Class

I changed my 3rd panel to be reactive on the x and y axis according to the input by the user, but i'm having an issue with an error and need to fix it. I included both sets of radio buttons that I want and I think it will look really cool once I figure out how to format it in a way that will work. 

## April 27th End of Class 

My 3rd panel is working after trouble shooting a bunch of stuff. I want to add another selectInput to include a second team option so you can compare two different teams in their respective statistics. I will figure that out and make the visualization look nice over the weekend. I'm happy about where my project is right now. 
