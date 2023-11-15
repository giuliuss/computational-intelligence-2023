# Lab 2: Nim ES

This code implements the game of Nim, where players take turns removing stones from a pile. The player who removes the last stone loses the game. The game can be played against the computer or against another player. The number of stones in the pile and the game mode are chosen by the user at the beginning of the game. The game ends when there are no more stones in the pile.

Each individual of population is characterized by a list of probability to use one of generic strategies and plays with others in order to define the best genotype of probabilities. 
After that, population is divided in two parts, only the first one will survive, will be duplicated and to the copy will be applied the crossover (mixing the genotypes) and the mutation.
After N trials, just pick the first genotype of the list, which have the best score of wins and let him playing with the optimal, pure random, gabriele and conservative strategies. 
As you can notice, he can't win lot of games against optimal strategy, but with others has many possibilities to win.

Final consideration: 
Don't think this is the best strategy to find a professional player, because the most important rule in nim game is to achieve a safe position and the various strategies don't consider that. 
A better solution may be use a list of pre-computed moves and valuate them after a good training. In that case, the player will have all the possible configurations of nim state and will choose the correct move to a safe one.