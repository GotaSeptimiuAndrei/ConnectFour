# 🎮 Connect 4 
 Connect 4 game built in python.

## How to play:
The two players take turns dropping colored tokens into a seven-column, six-row vertically suspended grid. The pieces fall straight down, occupying the lowest available space within the selected column. The objective of the game is to be the first to form a horizontal, vertical, or diagonal line of four of one's own tokens.

## Features:
- Console User Interface
-  Graphical User Interface, built with the Tkinter framework
- AI - implemented using the MiniMax Algorithm
- All modules with the exception of the UI are covered with specifications and PyUnit test cases
- Layered Architecture
- 2 strategies that can be used by the computer
- Customizable board size, initially set to standard: seven-column, six-row

## Settings
The users can change the game settings before launching the game (e.g., choosing between playing the game in the console or in a GUI, each player's name and whether they are controlled by an AI or not, and the strategy used by the AI for each player). This can be done by modifying the ```settings.properties``` file. The default settings are the following:
```
[DEFAULT]
ui_type = "GUI"
first_player_type = "Human"
first_player_name = "Yellow"
first_player_ai = ""
second_player_type = "Computer"
second_player_name = "Red"
second_player_ai = "Smart"
```
The ```ui_type``` can be either ```GUI``` or ```Console```, the types of each player can be ```Human``` or ```Computer``` and the AI type can be either ```Smart```, which employs a minimax strategy, or ```Random```, which chooses moves randomly.

## AI Implementation
The AI analyses every possible move from the current board state by using a minimax algorithm, trying to maximize the score of its moves and minimizing the score of the opponent's moves. In the case of this game, the score depends on the placement of the pieces and the possibilities of placing 4 pieces of one color in a row. The AI only simulates 3 moves in advance, since any more moves would seriously hurt the time performance. This way, it decides which move is the most profitable, and uses it once the computations are done. 

## Video sample (Human vs AI)
 <p align="center"> <img src="https://github.com/GotaSeptimiuAndrei/ConnectFour/blob/main/video.gif" height="500"/> </p>
