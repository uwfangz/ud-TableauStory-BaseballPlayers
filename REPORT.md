# Tableau Story Project
By Vicky Fang<br>

- Data after cleaning: [baseball_data_no_zero.csv](baseball_data_no_zero.csv)
- [First Version Story](https://public.tableau.com/shared/3G3Z7RD5G?:display_count=yes)
- [Second Version Story](https://public.tableau.com/views/BaseballPlayersData_story_final/Story1?:embed=y&:display_count=yes)
- [Final Version (revised)](https://public.tableau.com/views/BaseballPlayersData_story_final_rev1/Story1?:embed=y&:display_count=yes&publish=yes)
- [Summary](#summary)
- [Design](#design)
- [Feedback](#feedback)
- [Reference](#reference)

## Summary

This data set contains 1,157 baseball players including their handedness (right or left handed), height (in inches), weight (in pounds), batting average, and home runs. I’ve explored the data set first by visualizing the four measurements, *height,* *weight,* *batting average*, and *home runs*. Then I’ve explored the relationships between *batting average* and *home runs*. These explorations can all be filtered by the handness. 

## Design 

### Data Cleaning ###

As suggested by reviewer that "the players with batting averages of 0.0 are almost all pitchers, which generally don't go to bat", I decide to remove the players with batting averages of 0.0 since we cannot tell if the player is really bad at batting or he just never has a chance to bat. 

### Design Decisions ###

I want to tell a story of the relationship between batting average and home runs. Therefore, I first look at the *home runs* and *batting average* of the baseball players. I've used a bar graph here because it's easy to sort and allows me to compare the batting averages and home runs among players. Instead of looking at thousands of data, I've selected the top 20 players with the most home runs. Since *home runs* and *batting average* have different ranges of values, I've decided to show the mark labels. Average and median lines are also added so that users can compare each player with the rest of the players. 

After visualizing the performance of the top 20 players, I used histograms to describe the distributions of *home runs* and *batting average* of the entire data set. The bin size for the *Home Runs* histogram is set to 20. Since the range is from 0 to 563, I think 20 is appropriate sine I don't want the groups to be too coarse or too detailed. The bin size of the *Batting Average* is set to 0.0118. This time, I took the *"Suggest Bin Size"* value. I listed the range and bin size of the histograms in the captions to help users understand the graphs.  

To explore the relationship between *home runs* and *batting average*, I've used a scatter plot. A scatter plot is used to *"display values for typically two variables for a set of data"*. From the histograms of *home runs* and *batting average*, I've guessed that players with more home runs tend to have higher batting average because the batting averages of most top 20 players are distributed in the right part of the histogram. However, I'm not very sure about the relationship. With a scatter plot, I could display a trend line to see if there's a positive correlation between the two variables. To make the graph more interesting, I've also added *handness* as a filter. I want to see if there's a difference in the relationship when players are using different hands. I've used *highlight feature* on the legend so that users can click on a type of handness or a mark to highlight matching marks in the view.   

## Findings

First, I want to display the overall performance (by *home runs* and *batting average*) of the top 20 baseball players with the most home runs. I’ve displayed a bar graph, which viewers can use to look up the performance(s) of the baseball players.

Then I want to show the descriptive statistics of the two variables I'm interested in so that I can have an overview picture of the data. Thus, I've made histograms of *home runs* and *batting average*. After adjusting the bin size, I have a *Home Runs* histogram that's skewed to the right since most players have less than 50 home runs. I also have a *Batting Average* histogram that's skewed to the left. The most common batting average ranges from 0.24 to 0.27. According to Wikipedia, *"In modern times, a season batting average higher than .300 is considered to be excellent, and an average higher than .400 a nearly unachievable goal.”* This is consistent with my graph since we can see that there are few players having an average higher than 0.3. Then I've tried to see where the top 20 players would be distributed in the *Batting Average* histogram. I've found that most of them would be in the right side of the histogram, from 0.25 to 0. 28. Therefore, I have an assumption that players with more home runs tend to have higher batting averages.   

To check if my assumption is true, I explored the relationships between *batting average* and *home runs* using a scatter plot. I want to see that if batting average is positively related to home runs so I’ve added a trend line. From the scatter plot, I can see that although there is a positive correlation between the two measurements, the correlation is not very strong. I've also added the handness as a filter to the scatter plot. By selecting a handness, I can see that right-hand players and left-hand players have stronger correlations between *home runs* and *batting averages* that players using both hands.  

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

- [Batting average (baseball) Wikipedia](https://en.wikipedia.org/wiki/Batting_average_(baseball))
- [Home run Wikipedia](https://en.wikipedia.org/wiki/Home_run)
- [Reference Lines, Bands, Distributions, and Boxes](https://onlinehelp.tableau.com/current/pro/desktop/en-us/reference_lines.htm)
- [Creating a Reference Line which Appears and Disappears Based on a Condition](https://kb.tableau.com/articles/howto/creating-a-reference-line-which-appears-and-disappears-based-on-a-condition)
- [Scatter plot Wikipedia](https://en.wikipedia.org/wiki/Scatter_plot)
- [Legend Highlight](https://onlinehelp.tableau.com/current/pro/desktop/en-us/actions_highlight_colorlegend.htm)
