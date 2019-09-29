Hackathon - Pro Kabaddi League

Introduction:

Pro Kabaddi League is a professional-level kabaddi league that started in 2014. Currently, the League is in its 7th season, which started on 20 July 2019 with the first match between U Mumba and Telugu Titans. The final match will be played on 19 October 2019.
In this hackathon, task is to use coding and analytics skills to predict various outcomes at the end of the tournament.

Need to make predictions only for the current season of the tournament, i.e., season 7, but you are free to use the data from all the seasons.

Task 1: Predict the winner of the tournament

Task 2: Predict the top team in the points table after the completion of the league matches.

Task 3: Predict the team with the highest points for successful raids.

Task 4: Predict the team with the highest points for successful tackles. 

Task 5: Predict the team with the highest super-performance total.

Task 6: Predict the player with the highest SUCCESSFUL RAID percentage.

Task 7: Predict the player with the highest SUCCESSFUL TACKLE percentage.

Approach:

We've scraped data from multiple websites comprising of details of each team’s history in the season 5, season 6 and season 7 and have scraped the details of the fixtures of 2019 PRO kabaddi league as well. We stored the above piece of data in four separate csv files.

As the data from very first few seasons would not contribute much to current season as there were not many teams as current season, we have not considered it for training the model. So the data we've chosen seems to give a fairly good idea.

Then we performed cleaning of the data as per our needs to make a machine learning model out of it. We are using the current season ranking to predict the winner of the ongoing kabaddi league.

Ranking of teams are based on current season performance as these teams only play in Pro kabaddi league only. Fixtures are collected for rest of the tournament only as half of the season is already completed so we utilized current season data as well for testing.

Datasets were manually modified to include a row called “Team Value.” Team Value was measured by breaking down the 12 teams in the kabaddi league and dividing them into groups.

The first 3 teams on the standing were assigned a value of 5. The next four were assigned 4. The next four after that got a value of 3. Last four teams before relegation zone were assigned 2. Similar players were assigned a value based on their performnce in current and previous seasons.

Environment and tools:

Jupyter Notebook

Selenium webdriver

chrome driver manager

Beautifulsoup

Numpy

Pandas

Seaborn

Matplotlib

Scikit-learn

Websites used for Data Extract:

https://www.prokabaddi.com/

https://www.mykhel.com/kabaddi/pro-kabaddi/

Random forest and Linear regression was used to predict the outcome.
