# RootWinnerPredictor
Predicts the winner of a game of Root - 
Uses the dataset from round 1 of the 2021 Winter Tournament.
I have turned the data into binary for the purposes of classifcation, which is the CSV file.

When given a hypothetical game, the code will predict whether each player will win using kNN and going from 1 neighbors to 128.
However many total wins that player accumlates from the 128 tries are added up and presented as the total.
A more accurate way to describe the output is to say that the higher number means the most number of previous wins from someone in a similar scenario.

TO USE:
(1) Download the csv file and change line 7 of the code so the program accesses it. (2) The factions are abbreviated to the starting letter of the first two syllables, so type that in exactly when prompted. The map abbreviations are easier to interpret. Make sure to put the players in the correct seating order, the first faction you type will be considered the player with the first turn. (3) The player/faction with the most wins is considered "best". If all factions are at 0 points, it means there have been no similar situations to the one you have put in that have resulted in a win in any of the previous games.
