# TicTacToe.github.io
Created a Tic-Tac-Toe game using HTML ,CSS , Javascript and used minmax algorithm to make it unbeatable.
<br><br>
Tic-Tac-Toe is a simple, two-player game that, if played optimally by both players, will always result in a tie. The game is also called noughts and crosses or Xs and Os.
<br><br>
Rules: In a 3-by-3 grid game, the player who is playing "X" always goes first. Players alternate placing Xs and Os on the board until either player has three in a row, horizontally, vertically, or diagonally or until all squares on the grid are filled. If a player is able to draw three Xs or three Os in a row, then that player wins. If all squares are filled and neither player has made a complete row of Xs or Os, then the game is a draw.
<br><br>
About AI player: AI is used to play optimally against human player.In a two-player (A vs B) game, if player A scores x points (utility units), player B loses x points. Total gains/losses always sum up to 0.With that in mind, let’s proceed to the Minimax algorithm that’s suited for such cases.
<br><br>
Minimax is a kind of backtracking algorithm that is used in decision making and game theory to find the optimal move
for a player, assuming that your opponent also plays 
optimally. It is widely used in two player turn-based games such as Tic-Tac-Toe, Backgammon, Mancala, Chess, etc
<br><br>
Minimax algorithm: In layman's words,this algorithm sees a few steps ahead and puts itself in the shoes of its opponent. It keeps playing ahead until it reaches a terminal arrangement of the board (terminal state) resulting in a tie, a win, or a loss. Once in a terminal state, the AI will assign an arbitrary positive score (+10) for a win, a negative score (-10) for a loss, or a neutral score (0) for a tie.At the same time, the algorithm evaluates the moves that lead to a terminal state based on the players’ turn. It will choose the move with maximum score when it is the AI’s turn and choose the move with the minimum score when it is the human player’s turn. Using this strategy, Minimax avoids losing to the human player.
A Minimax algorithm can be best defined as a recursive function that does the following things:
1.return a value if a terminal state is found (+10, 0, -10)
2.go through available spots on the board
3.call the minimax function on each available spot (recursion)
4.evaluate returning values from function calls
5.and return the best value
