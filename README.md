# PythonProjects

Particle Labeling MLP:

The program is a classification agent that uses a combination of a multilayer perceptron (PyTorch implementation) and a support vector machine to accurately predict the labels for data points on a 2-dimensional plane. Some of the required specifications for the model included training the MLP on some training data with a small period of time (5 minutes max) and applying the prediction to a new data set. The ratio of correct vs incorrect labels was the measure of how well the agent did. This particular agent topped out a peak predict accuracy of 95.8%. While not runnable (code to run the program exists in the unknowing void of gradescope), the code itself serves as the demonstration. 

Adversarial Chess Agent:

Implements an adversarial search algorithm to decide what the best move would be in a modified version of chess. The fun part about this project is that as long as you have python3 installed on your computer, from Github you can download and run the code and have the agent play a match. The readme.txt file contains instructions on how to run it. 

The specific adversarial search algorithm the agent uses is mini-max with alpha beta pruning to improve efficiency. The program is given a maximum of 3 seconds to make a decision, any longer and the game is terminated and the other agent wins. The decision needs to be made very fast, so alpha beta pruning is used to increase the number of potential moves the agent can visit and access. 

Then comes the playout policy. The agent uses a complex scoring mechanism to assign each assessed move a score based on board position, opposing piece positions, and allied piece positions. In this modified version of chess (which really plays more like checkers), victory can be attained the moment an allied piece reaches the opponents back row. This is usually how the game is completed, though it is technically possible for the game to end with all the pieces being eliminated. 

As for attacking, every piece on the board is a pawn and can attack horizontally, or move horizontally even without an attack being executed if it is beneficial. While the agent does not always make the 100% best move all the time, the limited time span of a decision and slow speed of python make this problem difficult to tackle, though I'm sure with more time committed to the project the algorithm could be significantly improved. 

Details on how to run the program are in the folder itself. 
