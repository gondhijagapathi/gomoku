![icon](./images/Gomoku.png)

#### Compilation instructions ####

If you are on a linux machine, replace line number 2 of Makefile (CXX := clang++ -std=c++11 -stdlib=libc++) with 
```
CXX := g++
```
Run `make` in the project directory and you will find `pure_mcts_game` in the `bin/cppgomoku` directory.
To run the project, there are two required parameters. These are the two player parameters ('h' for human and 'c' for computer player ).
Below is an example where the game is played by two computer players.
```
./pure_mcts_game c c
```

The computer player’s best move is picked up using the Monte Carlo Tree Search algorithm where as the human player needs to provide his move using the [horizontal_index vertical_index] format.