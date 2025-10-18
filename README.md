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

The insight I have is that both Minimax and Alpha-Beta pruning work well with the Tic-Tac-Toe game, but if the game tree gets bigger, Minimax just becomes too slow. Alpha-Beta pruning, on the other hand, can handle larger trees more efficiently by skipping unnecessary branches, so it makes the AI faster while still playing perfectly. In conclusion, Alpha-Beta pruning is a more practical choice for complex games because it keeps the optimal decision-making of Minimax but significantly reduces the number of moves the AI needs to evaluate, making it both efficient and effective.

