# GameReinforcementLearning
Deep Reinforcement Learning in Tic-Tac-Toe Game: Machine Learning

A modified technique to train our policy network without training dataset of past games. Used ConvNet neural network to train a policy network using policy gradient method. Given a state of the game board policy network outputs best next move to make.

Policy gradient approach optimizes a policy given a function.

1) Function: The reward/score we get from the game we are playing given the actions we take

2) Policy: The choice of actions/moves playing the game

3) Input: Vector of nine elements representing Tic-Tac-Toe board with nine boxes.

4) Output: CNN network outputs the probability of a move in a given board position (Sotmax policy)

5) Better moves will result in more reward



Typically reinforcement learning methods use training set of past games to train neural networks. And these methods use tree search/min-max search algorithms to find best move/score/reward and use that as target for the policy network training.

Used two dueling networks learning from each other. So we do not require training dataset of past games. Inputs are random possible states of the board. And because of dueling policy networks reward/score function is a simple advantage function and does not require complex search algorithm as reward functions.

Advantages of this method are:

1) Unsupervised training: No past games data. Not using images of past games.

2) No labeled data for training

3) Simple advantage function for rewards

4) Learning by exploring various possible states in the game

Future work:

1) Fine tune back propagation and score function to speedup learning from dueling networks.

2) Use bigger machine with more RAM to use complex policy network.

3) Train on complex states as well. States with more number of moves.



See below link for more details:
https://www.linkedin.com/pulse/deep-reinforcement-learning-tic-tac-toe-game-machine-sarabjeet-singh
