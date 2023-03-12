# Tic Tac Toe Game
A simple Tic Tac Toe game created using HTML, CSS, and JavaScript.

## Getting Started
### Prerequisites
You only need a web browser to play this game.

### Installing
No installation is required. You can simply open the index.html file in your web browser and start playing the game.
You can also play the game via https://massl.codes/tik-tac-toe/

### Game Rules
The game is played on a 3x3 grid. Players take turns to mark a cell with their symbol (either X or O) until one player gets three of their symbols in a row, column, or diagonal, or until all the cells are filled, resulting in a draw.

### How to Play
Open the index.html file in your web browser
Click on any of the empty cells to place your symbol (X or O)
The game will automatically switch to the other player's turn after you have made your move.
Continue playing until a player wins or the game ends in a draw.
Click the "Restart" button to start a new game.
## Code Explanation
The game logic is implemented using JavaScript. The cells variable stores an array of all the cell elements, and the options variable stores an array that keeps track of the current state of the game board. The currentPlayer variable stores the current player's symbol (either X or O), and the running variable indicates whether the game is still in progress or has ended.

The game is initialized by calling the initializeGame() function, which sets up event listeners for the cell clicks and restart button, displays the current player's turn, and sets the running variable to true.

When a cell is clicked, the cellClicked() function is called. This function checks if the cell has already been marked or if the game has already ended, and returns if either condition is true. Otherwise, the function updates the cell with the current player's symbol and calls the checkWinner() function to see if the current player has won the game.

The checkWinner() function loops through all possible winning combinations and checks if any of them have been achieved by the current player. If a winning combination is found, the function displays the winner and sets the running variable to false. If all cells are filled and no winner is found, the function displays a draw and sets the running variable to false. Otherwise, the function switches the player by calling the changePlayer() function.

The restartGame() function resets all variables and cell contents to their initial state, and calls the initializeGame() function to start a new game.

### Author
This game was developed by Massinissa TAZEKRITT.
