# NBA Players Injury Analysis
Introduction
The NBA has changed from the early 90's. Players seem stronger, bigger and faster. Rules like hand-checking no longer exist, the 3 pointer has become a key focus to winning a championship(Golden State Warriors in 2014-15). One thing common in the NBA from then and now is injuries.
Injuries are detrimental to any team. When a Star Player gets injured the cost is not only potential wins but millions of dollars lost from injured players salaries and potential tickets sales. Fans don't want to pay for the price of admission to watch their star player on the bench in street clothes.
Kobe Bryant sustains Achilles Injury in 2013:
- miss 73 games
- Salary: 30,453,805 
- Cost to LA Lakers: 
    - 73  * 370,000/game = $28,000,000
Derrick Rose following MVP year sustains knee injury
- 2011-2014 Yearly salary: 17,632,688 Games missed: 43(2011), 82(all of 2012), 61(2013)  (knee injury)
    - Per game salary: roughly 215,000
    - Cost to team: ~ 40,000,000

# Goal
Create a list of key features that attribute to high injury rates. To do this I will focus on games played for each player in a season and Average per game Player stats. This list will help provide the coaching staff with insights/indicators to focus on monitoring the health of a player based on their stats and adjust accordingly to maximize games played in a season.

# Data Gathering
Scrape Regular Season NBA stats from NBA.com.
TRADITIONAL STATS
ADVANCED STATS
SHOOTING STATS
OPPONENT SHOOTING STATS
PLAYER BIOS
TEAM SCHEDULE GAME LOGS

# Approach
Divide the data into 3 separate blocks from 3 different eras. Each block consists of 5 years of NBA player data with attributes listed below. The target variable will be Games played per season. I want to analyze games played with the list of attributes using the following models: Linear Regression, Lasso, Ridge and Elastinet.

# EDA: Exploratory data analysis
I originally started with 67 different possible attributes. I Removed redundant variables like shot selection beyond 25 feet since 3 point stats were already included. Also, I removed high correlated variables with the use of a Heat map and Pairplot, narrowing down my attributes to 57.
3 Main blocks of data representing 3 different NBA eras.
datasets	5 years of accumulated data	Target
block1: Michael Jordan Era	1996-97, 1997-98, 1999-00, 2000-01, 2001-02	Games Played per player from 1996 to 2002
block2: Kobe Bryant Era	2004-05, 2005-06, 2006-07, 2007-08, 2008-09	Games Played per player from 2004 to 2009
block3: Lebron James Era	2010-11, 2012-13, 2013-14, 2014-15, 2015-16	Games Played per player from 2010 to 2016
(Excluding Lockout shortened NBA seasons 1998-99 and 2011-12)

