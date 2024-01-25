# Reinforcement-Learning
Demonstrated value iteration and Q-learning onto agents in a grid world, as well as simulated robot crawler and Pac-Man

This project was written in Python 3.6

To run gridworld and control the agent manually, run command:
python gridworld.py -m

To see a full list of options for running gridworld, run command:
python gridworld.py -h

To see a gridworld agent run with value iteration, run command:
python autograder.py -q q1

To play around and visualize the differences in policies depending on inputted MDP values, run command:
python gridworld.py -g DiscountGrid -a value --discount [YOUR_DISCOUNT] --noise [YOUR_NOISE] --livingReward [YOUR_LIVING_REWARD]

To manually control and watch Q-learning agent, run command:
python gridworld.py -a q -k 5 -m

To observe Q-learning agent with Epsilon Greedy action selection, run commands:
python gridworld.py -a q -k 100 --noise 0.0 -e 0.1
python gridworld.py -a q -k 100 --noise 0.0 -e 0.9

To observe the Q-learning crawler robot, run command:
python crawler.py

To make Pac-Man use Q-learning in order to complete the game, run command:
python autograder.py -q q5

If you want to see Pac-Man's Q-learning visually, run command:
python pacman.py -p PacmanQAgent -n 10 -l smallGrid -a numTraining=10

If you want to see Pac-Man use approximate Q-learning, run commands:
python pacman.py -p ApproximateQAgent -a extractor=SimpleExtractor -x 50 -n 60 -l mediumGrid
python pacman.py -p ApproximateQAgent -a extractor=SimpleExtractor -x 50 -n 60 -l mediumClassic
