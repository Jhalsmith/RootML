# RootML
This code has been a passion project of mine and I hope you will find it interesting. 

Explanation:

The code predicts both the winner and the final point total for a Root game based purely on the beginning set-up of the game.
The data I have used for this model are the data kindly provided by LilyG from MakeCraftGames from Rounds 1 & 2 of the 2021 Root Winter Tournament (RWT) organized by GuerricSamplesGames. This leads us to the biggest disclaimer of the model - the model is doing its best to predict based on the players and meta from the 2021 RWT which is different than broader public player base and meta.

Each player in a game is counted as a single obervation (or row) in the data. Thus, there are four observations per 4-player game of Root, and 256 total observations in the table. The player's entire set-up situation is marked down in binary in their observation. There are columns for whichever faction they are, and columns for the factions that their opponents are. The player's observation will have a 1 marked down for factions present, and a 0 marked down for factions absent. Likewise, they will recieve a 1 or 0 depending on the map used, and their seating position. There is a key

I have turned the data into binary for the purposes of classifcation, which is the CSV file.

When given a hypothetical game, the code will predict whether each player will win using kNN and going from 1 neighbors to 128.
However many total wins that player accumlates from the 128 tries are added up and presented as the total.
A more accurate way to describe the output is to say that the higher number means the most number of previous wins from someone in a similar scenario.

TO USE:
(1) Download the csv file and change line 7 of the code so the program accesses it. (2) The factions are abbreviated to the starting letter of the first two syllables, so type that in exactly when prompted. The map abbreviations are easier to interpret. Make sure to put the players in the correct seating order, the first faction you type will be considered the player with the first turn. (3) The player/faction with the most wins is considered "best". If all factions are at 0 points, it means there have been no similar situations to the one you have put in that have resulted in a win in any of the previous games.
