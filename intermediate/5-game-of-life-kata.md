## The Game of Life

Conways's Game of Life is a classic programming problem. In this game, a 2-dimensional grid of arbitrary size is filled with cells. These cells operate in a binary state: Alive or Dead. The cells then evolve based on a simple set of rules and the board changes with each passing time step.

## The Kata

Our job will be to create the model to calculate the next iteration for an arbitrary starting position of the Game of Life.

The board size is arbitrary, though traditionally square. In this first iteration, we'll assume that the edges do NOT wrap around, and that no life can exist beyond the edges of the board.

The cells will behave according to the following rules:
 1. Any live cells surrounded by fewer than 2 cells will die of loneliness.
 2. Any live cells surrounded by more than 3 cells will die of overcrowding.
 3. Any live cells surrounded by exactly 2 or 3 cells will remain.
 4. Any dead cells surrounded by exactly 3 neighbours will birth a new cell.

 ## Extending the kata

 Assume now that the game world is toroidal. That is to say that the edges will now wrap-around. Cells on the left 'edge' will be affected by cells on the right 'edge' and vice-versa. Similarily, cells on the top 'edge' will be affected by cells on the bottom 'edge' and vice-versa.


