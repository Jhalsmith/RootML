# RootWinnerPredictor
Predicts the winner of a game of Root - 
Uses the dataset from round 1 of the 2021 Winter Tournament.
I have turned the data into binary for the purposes of classifcation, which is the CSV file.

When given a hypothetical game, the code will predict whether each player will win using kNN and going from 1 neighbors to 128.
However many total wins that player accumlates from the 128 tries are added up and presented as the total.
A more accurate way to describe the output is to say that the higher number means the most number of previous wins from someone in a similar scenario.
