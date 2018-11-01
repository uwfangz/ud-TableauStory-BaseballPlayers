# Tableau Story Project
- Data: [baseball_data.csv](baseball_data.csv)
- [First Version Story](https://public.tableau.com/shared/3G3Z7RD5G?:display_count=yes)
- [Final Version Story](https://public.tableau.com/views/BaseballPlayersData_story_final/Story1?:embed=y&:display_count=yes)
- [Summary](#summary)
- [Design](#design)
- [Feedback](#feedback)
- [Reference](#reference)

## Summary

This data set contains 1,157 baseball players including their handedness (right or left handed), height (in inches), weight (in pounds), batting average, and home runs. I’ve explored the data set first by visualizing the four measurements, *height,* *weight,* *batting average*, and *home runs*. Then I’ve explored the relationships between *batting average* and *home runs*. These explorations can all be filtered by the handness. 

## Design

First, I want to display the overall performance (by *home runs* and *batting average*) of the baseball players in the data set. I’ve displayed a bar graph, which viewers can use to look up the performance(s) of the baseball players.

Then I want to show the descriptive statistics of the data set so that I can have an overview picture of the data. After connecting the data to Tableau, I know that I have the following dimensions and measures: *player name*, *handness*, *height*, *weight*, *batting average*, and *home runs*. I've made histograms of height and weight data. We can see that most baseball players in this data set weighs between 180 and 190 pounds. Most baseball players are from 72 to 74 inch tall. The most common batting average ranges from 0.2 to 0.3. According to Wikipedia, *"In modern times, a season batting average higher than .300 is considered to be excellent, and an average higher than .400 a nearly unachievable goal.”* This is consistent with my graphs since we can see that there are few players having an average higher than 0.3. 

Finally I’ve tried to explore the relationships between *batting average* and *home runs* using a scatter plot*.* I want to see that if batting average is positively related to home runs so I’ve added a trend line. Since batting average *“**is defined by the number of hits divided by at bats**”*, I assume that players with higher batting average would hit more home runs. From the scatter plot, I can see that although there is a positive correlation between the two measurements, the correlation is not very strong. 

**Changes made after [feedback](#feedback)**

After receiving feedback from a friend, I’ve added the following components into the design of the visualization:

- Added more interactions into the first slide; viewers can now specify number of players to display and toggle average and median lines for home runs and batting average respectively to compare the performance of the players. 
- Allowed trend lines per color so that viewers can compare the performance among players with different handness. 
## Feedback

***What do you notice in the visualization?***

The graphs are titled and annotated. The visualization is overall clear; there are 2 histograms for the *height* and *weight* measurements; there are 2 line graphs for the *batting average* and *home runs* measurements. I can use the *handness* filter to see the compare the graphs under different conditions of *handness.* There’s also a scatter plot to explore the relationship between *batting average* and *home runs*. 

***What questions do you have about the data?***

- Which player has the most home runs?
- Which player has the highest batting average?
- Are players with higher batting average more likely to have more home runs?
- Do players with right handess tend to hit more home runs than players with left handness?

 
***What relationships do you notice?***

*Batting Average* is positively correlated with *home runs*, although the relationship is not very strong. I’d like to see the trends lines among players with different handness so that I can compare them.  

***What do you think is the main takeaway from this visualization?***

The main takeaway is that home runs are positively correlated with batting averages, although the relationship is not very strong. Home runs hit by baseball players with right handness have slightly stronger correlations with their batting averages than the players using left hands or both hands. 

***Is there something you don’t understand in the graphic?***

The title of the story is *Differences among the performance of the baseball players*. However, I haven’t see any comparison of the performance among different baseball players. I think the story would be better if you can add some comparisons of the performance. 


## Reference

- [Batting average (baseball)](https://en.wikipedia.org/wiki/Batting_average_(baseball))
- [Home run](https://en.wikipedia.org/wiki/Home_run)
- [Reference Lines, Bands, Distributions, and Boxes](https://onlinehelp.tableau.com/current/pro/desktop/en-us/reference_lines.htm)
- [Creating a Reference Line which Appears and Disappears Based on a Condition](https://kb.tableau.com/articles/howto/creating-a-reference-line-which-appears-and-disappears-based-on-a-condition)
