# QuoridorAI

This is an AI agent who plays Quoridor board game

## If you want to play against our agent:
First you'll have to run our agent on a port 
```
python my_player.py --bind localhost --port 8000
```
You can replace the port 8000 by one of your choice if 8000 is already used.
Once it is done, you can now start a game by running this command
```
python game.py http://localhost:8000 human --time 300
```
#### Note: http://localhost:8000 is the adress on which you executed our player, don't forget to put the same port number than the previous command. Also the time option of 300 seconds means our agent have 300 seconds to use throughout the game, you can change it but keep in mind that this will affect the performance of our agent and therefor make it easier for you.

## If you feel too lazy to play
Just had a long day or don't even know the rules ? You can still watch a fun game of quoridor while eating.
You can watch our agent perform against two other agent.
```
python my_player.py --bind localhost --port 8000
```
#### Run the opponent. Either random_player.py OR greedy_player.py. Make sure to use a different port than the one for my_player.py
```
python random_player.py --bind localhost --port 8080
```
And now you can watch the game 
```
python game.py http://localhost:8000 http://localhost:8080 --time 300
```
