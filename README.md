[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=21115847&assignment_repo_type=AssignmentRepo)

# Minimax Tic-Tac-Toe Documentation

## What is Minimax?

The Minimax algorithm is used in two-player games where players take turns making moves. One player tries to maximize their chance of winning, while the other tries to minimize it. The algorithm explores all possible moves recursively, simulating each player’s turn, and assigns scores to terminal states: +1 for a win, -1 for a loss, and 0 for a draw. By working backward from these scores, Minimax chooses the move that guarantees the best outcome, assuming both players play optimally. This way, the AI can plan ahead and respond to every possible move of the opponent.

## How it Works

1. **Game Tree**: Creates a tree of all possible game states
2. **Recursive Search**: Explores every possible move from current position
3. **Scoring**: Assigns values to terminal states (win/lose/draw)
4. **Backtracking**: Works backwards to find the best move
5. **Optimal Play**: Guarantees the best possible outcome

## Alpha-Beta Pruning

Alpha-Beta pruning improves Minimax by keeping track of the best values for MAX (α) and MIN (β) and skipping branches that cannot influence the final decision. This reduces the number of nodes explored, so the AI can make decisions faster without losing optimal play.

### Performance Impact:
- **Without pruning**: Evaluates all possible game states
- **With pruning**: Cuts off unnecessary branches
- **Result**: Faster decisions with same optimal play

## Reflection

From my research po and insight is that both Minimax and Alpha-Beta pruning work well for the Tic-Tac-Toe game but if the game is too complex mas mahihirapan po or mababagalan yung Minimax so much better po gamitin doon yung Alpha-Beta Pruning po because of the features po na pag skip or pruning if nakita na na or na calculate na mas bababa ang chance na i pick po ito ng Player.

