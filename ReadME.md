## Project Goal
This project aims to make predictions to help choose an optimal fantasy roster in a Draft Kings classic NBA tournament.  Draft Kings is a daily fantasy site where users can wager and win real money.  The tournament this project takes into consideration is a classic NBA tournament.  The user has a hypothetical $50,000 "salary cap" to use on their roster.  The roster is made up of 8 players who's "salary" can range from $3,000 to $10,500.

This task was tackled by building both regression and classifier models.

## Notebooks

The entries in this repo should be viewed in this order:

- Technical Report
- 01 - Data Gathering
- 02 - Models

The Data Gathering notebook displays the code used to web scrape all of the data from nba-reference.com.  It would be helpful to view either the game log or advanced game log page for any player to follow along with what the web scraping code is accomplishing.  Every 20 rows the column names are repeated in the table, so code was written to skip those rows.  Code was also written to skip rows that represented a game in which a particular player did not play.

More than three regressor and more than three classifier models were considered, but the ones displayed in the 02 - Models notebook had slightly better performance than any others that were considered. Given more time and computing power I may have done more grid searching for optimal hyper parameters.

I fit a LinearRegression model, a RandomForestRegressor model, and a GradientBoostingRegressor for the regression problem and a RandomForestClassifier, GradientBoostingClassifier, and a LogisticRegression model for the classification problem.
