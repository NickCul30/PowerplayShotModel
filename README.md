
<h2>Powerplay Shot Model</h2>

Using the NHL Game Dataset from <a href="https://www.kaggle.com/datasets/martinellis/nhl-game-data?select=game_plays.csv">kaggle</a>, the game_plays.csv dataset was used to train a model to predict the number of shots a team will get on a Powerplay oppurtunity. In it's current state the model can predict the number of shots taken with about a 45% accuracy.

The model was trained on years worth of NHL games, and per powerplay was given the following data to use :
- Which teams were on the PP / PK
- Game index (indexing game and season)
- Period and time
- Current score of the game

In-order for the training data to be correct a few rules had to be followed :
- Powerplays last 2 minutes of game time
- A goal ends a powerplay
- Another penalty ends a powerplay

Improvements that can be made :
- Only minor penalties were used
- Penalties awarded in the last two minutes of a period/game were not used
- 5 on 3 powerplays are not detected
- Model can't detect when penalties offset
