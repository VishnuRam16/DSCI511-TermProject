# DSCI511-TermProject

# NBA Players and Teams Stats through 2013-2021

<b> Team Members </b>
  - Vishnu Ram Murali
  - Mohammed Shehaf Aakil Sharfudeen
  - Varun Sharma
  - Sukhmani Kaur Mangat
  - Abhishek Patil

<b> API used </b>
- Sport Radar API

<b> Files and Documents </b>
1.	player_stats_data-2.ipynb – Python file that acquires data for player statistics from 2013 to 2021
2.	team_stats_final_data-2.ipynb – Python file that cleans, formats and merges team_wins_by_year.csv and team_yearly_stats_final.csv
3.	project_1-3.ipynb – Python file that acquires data for team statistics from year 2013 to 2021
4.	Team_Wins_By_Year.ipynb – Python file that acquires data for team win and loss by year from 2013 to 2021 
5.	player_yearly_stats_data.csv – Dataset that contains player statistics from 2013 to 2021
6.	team_wins_by_year.csv – Dataset that contains team wins and loss statistics from 2013 to 2021
7.	team_yearly_stats_final.csv – Dataset that contains all NBA teams statistics from 2013 to 2021
8.	Yearly_NBA_Team_Stats_Data1.csv – Final merged dataset of team_yearly_stats_final.csv and team_wins_by_year.csv

<b> How the dataset was created </b>

To obtain the key to access the data via the API, we create an application at sport radar. After generating the key, we request data from sport radar through the API. Because the raw data is nested in a dictionary and has multiple branches, we must carefully read the documentation to extract the correct set of data.

<img width="468" alt="Picture1" src="https://user-images.githubusercontent.com/49813115/205524125-129db390-f506-4284-a595-3ac91ab41433.png">

Then we write a function that takes the year, teamid, and key as parameters and returns a dictionary of data with all of the desirable attributes. The URL allows you to change the year, teamid, and key. As a result, we can easily obtain data for all 30 NBA teams from 2013 to 2021. To reduce run time and potential data loss, we create four separate datasets and then merge them into one. Some of the attributes are self-explanatory, but we will define some to make the data easier to understand.

<b>Position:</b> Basketball is a team sport with five players assigned to positions. From a strategic standpoint, these players have traditionally been assigned to positions defined by the role they play on the court. Guard, forward, and center are the three main positions, with a standard team consisting of two guards, two forwards, and a center. As more specialized roles emerged, the guards and forwards became differentiated, and today each of the five positions is known by a unique name, as well as a number: point guard (PG) or 1, shooting guard (SG) or 2, small forward (SF) or 3, power forward (PF) , Forward (F) or 4, and center (C) or 5.

<b>Turn Over:</b>
A turnover occurs when a team loses possession of the ball to the opposing team before a player takes a shot at their team's basket.

<b>Turn Over Ratio:</b>
Turnover Ratio, also known as turnover percentage, is the percentage of a team's or player's possessions that end in a turnover. Calculating the number of turnovers a player will make in 100 possessions makes itself 'tempo-free' (adjusted for team pace and minutes played) NBA stats that everyone wants to look at.

<b>Free Throw:</b>
A free throw is a special type of shot that's awarded to a player who gets fouled. They go to the foul (or “free throw”) line, which sits 15 feet from the basket, and shoot either one, two, or three free throws depending on the situation. Every shot the player makes is worth one point.

<b>Personal Fouls:</b>
Any player whose actions against an opponent cause illegal contact with yet another opponent has committed the personal foul. A personal foul committed by the offensive team during a throw-in shall be an offensive foul, regardless of whether the ball has been released.

<b>Technical Team Fouls:</b>
In basketball, a technical foul (colloquially known as a "T" or a "tech") is any infraction of the rules penalized as a foul which does not involve physical contact during the course of play between opposing players on the court, or is a foul by a non-player.

<b>Flagrant Fouls:</b>
A flagrant foul is a personal foul that involves excessive or violent contact that could injure the fouled player. A flagrant foul may be unintentional or purposeful; the latter type is also called an "intentional foul" in the National Basketball Association (NBA). However, not all intentional fouls are flagrant fouls, as it is an accepted strategy to intentionally commit a foul (without intent to injure) in order to regain possession of the ball while minimizing how much time elapses on the game clock.

<b>Minutes:</b>
Minutes – the total number of minutes a player is in the game. To track this accurately you must make substitutions at the correct clock time.

<b>Points:</b>
Points in basketball are used to keep track of the score in a game. Points can be accumulated by making field goals (two or three points) or free throws (one point). If a player makes a field goal from within the three-point line, the player scores two points. If the player makes a field goal from beyond the three-point line, the player scores three points. The team that has recorded the most points at the end of a game is declared that game's winner.

<b>Second chance points:</b>
A second chance point in basketball is when a team scores off a missed basket from their own player. Being able to score from a miss on the first attempt.

<b>Points Against:</b>
PA stands for Points Against. It is determined by adding up the total amount of points that were scored by your opponents each week.

<b>Rebound:</b>
A rebound, sometimes colloquially referred to as a board is a statistic awarded to a player who retrieves the ball after a missed field goal or free throw.

<b>Two Pointer:</b>
The most common type of scoring in basketball is the 2-point basket. This is any shot that is made from inside of the 3-point line (22 feet) and can be done with a jump shot, layup or dunk.

<b>Three Pointer:</b>
The second most common type of scoring in basketball is the 3-point basket. This is any shot that is made from outside of the 3-point line (22 feet).

<b>Steal:</b>
A steal occurs when a defensive player legally causes a turnover by their positive, aggressive action(s). This can be done by deflecting and controlling, or by catching the opponent's pass or dribble of an offensive player. The defender must not touch the offensive player's hands or otherwise a foul is called.

  <b>Blocked attempts:</b>
For the shooter, a blocked shot is counted as a missed field goal attempt. Also, on a shooting foul, a blocked shot cannot be awarded or counted, even if the player who deflected the field goal attempt is different from the player who committed the foul.



