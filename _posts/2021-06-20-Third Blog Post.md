---
layout: post
title: Third Post- Project 1- Creating a vignette about functions to read and analyze data from the NHL records API
---
In this project, I was given the task of creating a vignette that reads data from the [NHL records API](https://gitlab.com/dword4/nhlapi/-/blob/master/records-api.md) 
(using functions from the `httr` and `jsonlite` packages) and shows some basic exploratory data analysis using tools available in the `tidyverse` package and others.

I initially created functions to contact the NHL records API for 6 endpoints using the `jsonlite` package. These functions return data frames, with all of them using
ID (franchise ID or team ID) as arguments. However, the user has the option to use both ID and team full name to access the season records, goalie records, skater records
and franchise detail. A function was also written to access the NHL Stats API. Mapping the team names to their IDs was somewhat challenging, and took a while to figure out.
It was pretty straightforward after realizing the `which` function could be used. I then wrote a wrapper function to access all the API endpoints.

Using the wrapper function, data sets, numeriical summaries and new created variables and tablees were created. Some plots were also generated using `ggplot`. While I don't usually
follow the NHL, some interesting trends were observed: 
* Centers for the Dalllas Stars tend to spend the least time in the penalty box while defenders spend the most. 
* Teams that perform well at home during the regular season do well at home during the playoffs as well. 
* Home advantage did not really count for much when the _percentage_ home wins were compared to the percentage road wins during the regular season. (The wins were calculated
  as win divided by the sum of win, draws and losses).
* Defenders tend to spend the longest time with the Dallas Stars, although most players spent 5 seasons or less. 
* Teams that are very aggressive also have the best defensive solidity and vice-versa.

Working on the project took the better part of a week, mainly because of the time spent trying to understand the APIs and how to correcting write the functions (I've never written more than two nested `if` or `if else` statements before.) The task was also executed using the limited knowledge I have of R so far, it will be interesting  to learn better ways of writing the codes for this project as the semester progresses.

Overall, this project further increased my familiarity with R. It was pretty rewarding to be able to pull data from APIs and gain some insight. It's something I'll definitely be
interested in doing more of whether or not my career leads me down the data scientist path.

[Github repo](https://github.com/yemoray/ST-558-Project-1)  
[Github page](https://yemoray.github.io/ST-558-Project-1/)




