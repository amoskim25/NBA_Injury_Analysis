# NBA Players Injury Analysis
The NBA has changed from the early 90's to now. Players seem stronger, bigger and faster. Rules like hand-checking no longer exist and the 3 pointer has become a key focus to winning a championship. One thing common in the NBA from then and now is player injuries. Injuries are detrimental to any team. When a star player gets injured the cost is not only potential wins but millions of dollars lost from the player's salary and potential ticket sales. Sports fans do not want to pay expensive admission prices to watch their star player on the bench in street clothes.

Kobe Bryant sustains Achilles Injury in 2013:
- miss 73 games
- Salary: 30,453,805 
- Cost to LA Lakers: 
    - 73  * 370,000/game = $28,000,000
Derrick Rose following MVP year sustains knee injury
- 2011-2014 Yearly salary: 17,632,688 Games missed: 43(2011), 82(all of 2012), 61(2013)  (knee injury)
    - Per game salary: roughly 215,000
    - Cost to team: ~ 40,000,000

## Goal
Create a list of key features that attribute to high injury rates. To do this I will focus on games played for each player in a season and Average per game Player stats. This list will help provide the coaching staff with insights/indicators to focus on monitoring the health of a player based on their stats and adjust accordingly to maximize games played in a season.

## Data Gathering
Scrape regular season NBA stats from NBA.com including: Traditional stats, Advanced stats, Shooting stats, Opponent Shooting stats, Player Bio stats, Game Log stats

## Approach
Divide the data into 3 separate blocks from 3 different eras. Each block consists of 5 years of NBA player data with attributes listed below. The target variable will be Games played per season. I want to analyze games played with the list of attributes using the following models: Linear Regression, Lasso, Ridge and Elastinet.

## EDA: Exploratory data analysis
I originally started with 67 different possible attributes. I removed redundant variables like shot selection beyond 25 feet since 3 point stats were already included. Also, I removed high correlated variables with the use of a Heat map and Pairplot, narrowing down my attributes to 57.
3 Main blocks of data representing 3 different NBA eras.
datasets	5 years of accumulated data	Target
block1: Michael Jordan Era	1996-97, 1997-98, 1999-00, 2000-01, 2001-02	Games played per player from 1996 to 2002
block2: Kobe Bryant Era	2004-05, 2005-06, 2006-07, 2007-08, 2008-09	Games played per player from 2004 to 2009
block3: Lebron James Era	2010-11, 2012-13, 2013-14, 2014-15, 2015-16	Games played per player from 2010 to 2016
(Excluding lockout shortened NBA seasons 1998-99 and 2011-12)

# Conclusion
The top 5 attributes associated with games played across all three eras are:
- Average Minutes
- Win-Percentage
- Personal Fouls
- True-Shooting Percentage
- Age

The takeaway to this research is to provide more insight on injuries. A coaching staff would monitor a player's minutes played and adjust according to age. Also, win-percentage and true-shooting percentage are indirectly correlated to injuries.


