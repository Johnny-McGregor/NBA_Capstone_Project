## Project Goal
This project aimed to see if it can make predictions that would help someone choose an optimal fantasy roster in a Draft Kings competition.  This task was tackled by building both regression and classifier models.

##Notebooks
The two notebooks in this repo should be viewed in this order:
- 01 - Data Gathering
- 02 - Models

The Data Gathering notebook displays the code used to web scrape all of the data from nba-reference.com.  It would be helpful to view either the game log or  advanced game log page for any player to follow along with what the code is accomplishing.  Every 20 rows the column names are repeated in those tables, so code was written to skip those rows.  Code was also written to skip rows that represented a game in which a particular player did not play.

More than three regression and more than three classifer models were considered, but the ones displayed in the Models notebook had slightly better performance than any others that were considered. Given more time and computing power I may have spent more time Grid Searching for optimal hyper parameters.
