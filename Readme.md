
### Project Description
The project is about a website that is made for people who are cricket enthusiasts and people looking
to debate each other on who’s a better player or a team. The website displays ball by ball (granularity of the data) player statistics
and gives it in the form the user wants, be it searching for speciﬁc players, or teams, or simply team statistics, balling statistics,
batting statistics, the top players in each aspect, and a lot more. We have a robust database design with the appropriate constraints and 
triggers, so that users can add data as well.

### How to Build this project  (basic working knowledge of nodejs projects expected)
  1. Install npm, and postgresql.
  2. Install the required packages of npm for express, ejs etc.
  3. Download the project.
  4. Build node modules folder using npm init.
  5. Make your local postgres database using the databse provided as a link in next portion.
  6. use the create_table sql file to make the tables, views and triggers.
  7. Configure your database in the app.js file.
  8. Run the app.js file and open the localhost in your browser.


### Data Sources and Statistics
We downloaded our dataset from https://www.kaggle.com/raghu07/ipl-data-till-2017. The data was available in .csv format.
So we directly downloaded it and analyzed it using MS Excel. The date was structured but it was not clean.
We obtained our data from https://www.kaggle.com/raghu07/ipl-data-till-2017. This contains the data of all IPL seasons from 2008 to 2017 on a ball by ball granularity.
The data was availabe on the website in csv format. Minor pre-processing steps were taken such as removing the characters that were not UTF encoded,
but not much because the datasets present on kaggle are mostly clean and ready to be used. 


**Entity       -    Attributes**

**team**       -   team id,team name 

**player**     -  player id, player name, dob, batting hand, bowling skill, country name

**match**      -  match id, team1, team2, match date, season year, venue id, toss winner, match winner, toss name, win type, outcome type, manofmatch, win margin

**ball**       -  match id, over id, ball id, innings no, striker batting position, extra type, runs scored, extra runs, out type, striker, non striker, bowler, player out, ﬁelder
