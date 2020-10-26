# Fintech Group Project #2
## ASU Fintech Fall 2020 Course
### Group 1:
 * Sheldon Harracksingh
 * Xavier Spurlock
 * Richard Ripley
 
 # Betting on the 49ers game Total Score
 ---
![San Francisco 49ers](https://images2.minutemediacdn.com/image/fetch/w_736,h_485,c_fill,g_auto,f_auto/https%3A%2F%2Fninernoise.com%2Fwp-content%2Fuploads%2Fgetty-images%2F2020%2F09%2F1272315795-850x560.jpeg)

**Objective**: Predict the total score week-by-week for the San Francisco 49ers game in order to more accurately bet on the Over/Under line. 

**What does OVER/UNDER Mean in Betting?**
OVER/UNDER betting is also called a totals bet. The total in any given sporting event is a combined score of both teams. The total for these games is an amount that is set by oddsmakers based on how they envision a game will unfold from a scoring perspective. As a bettor, you would need to select if the total number of points scored by both teams will be OVER or UNDER the set total.
 - via [oddshark.com](https://www.oddsshark.com/sports-betting/over-under-betting)

**Methodology**: In order to achieve our goal, we wanted to implement Machine Learning via Turicreate to run Linear Regression and Boosted Trees Regression. The links below are where we aquired our data. 
* https://en.wikipedia.org/wiki/List_of_current_National_Football_League_stadiums
* https://www.pro-football-reference.com/teams/sfo/
* http://www.aussportsbetting.com/data/historical-nfl-results-and-odds-data/

**Target** = Total Score (Home score + Away Score). 

**Features** = Home Team, Away Team, Total Score Open, Location, Surface, Roof type, Game Time, GameDay, Month, Year

 - **Why *these* features?**
There are a total of 32 NFL teams, all located in varying cities/stadiums. Each game can be played at varying times and on different kinds of turf (i.e. grass vs. artificial). Without knowing each week’s betting line, or final score months in advance, these consistent features were utilized to best predict future outcomes. The machine should learn that the game day, time, location, and even time of year, all play an important role in determining total score. 

**Results**: Our model backtested by predicting the total scores of random, previously played games.

 - Total Score (Open Betting Line):
[52.0, 46.0, 48.0, 46.0, 39.5, 46.5, 42.5, 45.5, 46.0]

 - Model Prediction:
[53.3, 49.7, 44.8, 50.46, 30.3, 13.8, 47.2, 48.5, 47.8]

 - Actual Scores:
[60, 44, 47, 37, 29, 50, 32, 55, 41]

 - Max Error: 
36.16341209411621

 - RMSE: 
14.500893276625948

 - Future game prediction: 
10/25 Niners at Patriots 

   - Open betting line: 
44.5

   - Model Prediction: 
47.9

**Conclusion**:

We realize with more time and more features, our model may be able to better predict NFL total scores for all games, not just the 49ers. Once it learns week-by-week from it's successes and failures, we could hopefully train the model to better weigh the values of certain features. For example, we feel as the current season goes deeper into the Fall/Winter portion, the Game Time, Turf type, Roof type, and Location could all play a bigger role once the weather gets less favorable. Some things we could add in the future are actual team statistics to better compliment our data features for increasingly more reliable outcomes. 