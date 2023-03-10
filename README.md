# dream11-team-combination

## Fantasy Cricket Team Combination Generator
This code generates 20 random combinations of 11 players each for a fantasy cricket team. The player data is read from a CSV file, and the players are ranked based on their predicted performance, current form, and popularity among other fantasy cricket players.

## Requirements
pandas
random
Usage
Ensure that the required libraries are installed.
Download the match2.csv file to the same directory as the script.
Run the script.
The script will generate 20 random combinations of 11 players each and display their total ranking. Each combination is selected based on the players' predicted performance, current form, and popularity among other fantasy cricket players.

## How it works
The player data is read from the match2.csv file using the pandas library.
Any ranges of two values in the 'predicted_performance' column are converted to the average of the two values.
Any invalid values in the 'predicted_performance' column are replaced with the mean of the column.
The 'predicted_performance', 'form', and 'dream_team_percentage' columns are converted to numeric data type.
Any rows with missing data or null values are dropped.
A new column 'rank' is created by calculating the weighted average of the 'predicted_performance', 'form', and 'dream_team_percentage' columns.
The dataframe is sorted based on the 'rank' column in descending order.
20 random combinations of 11 players each are generated by randomly selecting players from the sorted dataframe.
Each combination is ranked based on the total ranking of the selected players.

## Disclaimer
This code is intended for educational purposes only. The rankings generated by this code are not a guarantee of actual player performance and should not be used for gambling or other purposes.
