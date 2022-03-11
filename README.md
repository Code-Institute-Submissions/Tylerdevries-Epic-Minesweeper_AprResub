# EPIC MINESWEEPER 

Epic Minesweeper is a python terminal game, which runs in the Code Institute mock terminal on Heroku

Users play a game of randomized minesweeper where if they dig in the wrong row and column comboniation they will blow up. 

Here is a live version of the site: https://epic-minesweeper.herokuapp.com/


![responsive mine](https://user-images.githubusercontent.com/93283135/157785203-fbd34013-75e1-4375-81b4-fc86c76529a1.PNG)

## How to Play

Epic Minesweeper is a game heavily influenced by the classic game minesweeper. You may have played it if you own a windows computer, but if not you may read up on the rules and history on wikipedia: https://en.wikipedia.org/wiki/Minesweeper_(video_game)

In this version, when the python is deployed a randomized board appears.

It prompts the user to dig by entering an input in the format of row,column.

The board has 9 rows and 9 columns meaning there is 81 possible inputs. 

The top left is 0,0 and the bottom right is 9,9

The user digs until they hit a bomb or clear the board, leaving just the bombs.

## Features

### Existing Features

Random board generation:

* Bombs are randomly placed throughout the board.
* User cannot see these bomb until they have dug.
* The game prompts the user to dig via input.
* The game guides the player with the necessary format for the input.


![beginning screen](https://user-images.githubusercontent.com/93283135/157786413-a9d49d56-675e-4ede-b52f-46ddd4b596b8.PNG)

Input:

* When the user enters their input the board will appear again.
* It may display a GAME OVER with an x where the user dug marking the existence of a bomb.
* It may also display a number where the user dug representing how many bombs neighbour that site.
* If no bombs are neighbouring the site, the site becomes 0, and all adjacent sites will be recursively revealed.
* The game now prompts the user to try again.
* If the user inputs the same site it was just repeat the board.
* When the board is cleared the player wins and will be prompted with a message saying WINNER!!!

![image](https://user-images.githubusercontent.com/93283135/157787566-4560e1b4-a343-488d-ac04-347828f6f4bc.png)

### Future Features:

* Create a way for the player to mark sites they know contain a bomb
* Create a difficulty mode
* Create a way to track high scores via time.

## Data Model

I used a Board class to create the field for the game. 

This class stores and creates the location of the bombs on the field, the guesses and the adjacent bombs. 

The class has methods to help play and display the game, such as the print method which displays the current board after each input.

## Bugs 

### Solved Bugs

* When I originally wrote the project I was getting constant indentation errors due to trying to fit functions inside the 80 character limit. I took help from users on stack overflow to remedy this issue by properly indenting my functions using parenthesis. 

### Remaining Bugs 

* There are no remaining bugs. 

### Validator Testing

PEP8: No errors returned. 

## Deployment

This project was deployed using Code Insitutes mock terminal for Heroku.

Steps for deployment:
* Fork or clone the depository
* Create a new Heroku app
* Set the buildbacks to python and NodeJS in that order
* Link the Heroku app to the repository
* Click on Deploy

## Credits

* Code Institute for the deployment terminal.
* Wikipedia for details on minesweeper
* http://ami.responsivedesign.is/ for the image of the app on seperate devices.













