## Tic-Tac-Toe Optimization

Tic-Tac-Toe is a classic strategy game where two players take turns marking X's and O's on a 3x3 grid until one player gets three in a row, either horizontally, vertically, or diagonally.

This optimization adds the case of an AI player to the existing game and implements the alpha-beta pruning algorithm to improve the AI's decision-making process.

## Implementation 
The code is an implementation of the alpha-beta pruning algorithm for a two-player zero-sum game. It calculates the optimal move for a player in a game by using a minimax algorithm with alpha-beta pruning and memoization to reduce the number of states that need to be evaluated. The algorithm is applied recursively and a value of the game state (value) and precision of the calculation (precise) is returned.

It contains several helper functions to support the main alpha-beta function:

- utility: calculates the value of a given game state.
- shuffled: shuffles an array randomly.
- hash: generates a unique string representation of a given game state.
- alphabeta: the main implementation of the alpha-beta algorithm.

The inputs to the alphabeta function include:

- state: the current state of the game board.
- depth: the depth limit of the search.
- alpha and beta: the cut-off values for the alpha-beta pruning.
- maximizingPlayer: a boolean value indicating whether the first move should be maximizing.
- counter: a counter to keep track of the number of calls to the alphabeta function.
- memo: a dictionary used to store the results of the game state values, which can be reused to reduce the number of state evaluations.
## How to Play
The game can be played in two modes: human-vs-human and human-vs-AI. In the human-vs-human mode, two players take turns marking X's and O's on the 3x3 grid. In the human-vs-AI mode, one player plays as X's and the other player is the AI, which uses the alpha-beta pruning algorithm to make its moves.

## Alpha-Beta Pruning
Alpha-beta pruning is a widely used search algorithm in game theory and AI. It is used to reduce the number of nodes that need to be evaluated in the search tree. The algorithm uses two values, alpha and beta, to keep track of the best possible move that the current player can make, as well as the best possible move that the other player can make. This information is used to determine whether or not it is worth evaluating a particular node in the search tree.

## How to Use
To run the game, simply run the main script file. The game will prompt you to select the mode of play, either human-vs-human or human-vs-AI. If you select the human-vs-AI mode, the game will also ask you to select which player you would like to be.

## Conclusion
This optimization adds a new level of challenge to the classic Tic-Tac-Toe game by introducing an AI player that uses the alpha-beta pruning algorithm to make its moves. Whether you are a seasoned player or new to Tic-Tac-Toe, this optimization offers an exciting new way to play the game.

