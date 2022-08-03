# NEAT-Missile-Guidance <br>
Winning submission to Fujitsu HelloAI Hackathon 2018. Video submission: https://www.youtube.com/watch?v=ogi5huhrmlk <br>
<br>
Abstract
Welcome to our NEAT python notebook!

This notebook lays out a framework to solve problems using the NEAT algorithm - based on this paper by Kenneth O. Stanley and Risto Miikkulainen: http://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf

The example we use in this notebook is that of a 2D missile guidance problem, but the framework has been made to plug in any potential problem that can be solved by NEAT.

The NEAT algorithm is a type of NeuroEvolutionary algorithm - one which we evolve artificial neural network (ANN) topologies over a series of generations to find an ANN that can solve our problem. Evolutionary learning is an untraditional but effective way to train a neural network to solve certain tasks. Tasks that are suitable to be solved by NeuroEvolutionary algorithms are ones where the success of the network is measured over a series of moves. This differs from networks that we train by more conventional methods such as back-propogation as these networks require supervision on every 'move' they make.

It would be unsuitable to use NEAT to train a neural network to solve a classification task, because every training move requires supervision, a yes or no answer. It would be much more effective training a network like this using traditional methods such as back propogation. Tasks that should be solved by an ANN trained with NEAT are tasks where the success of each ANN can only be measured over a series of moves, because each individual move does not have a right or wrong answer. For example, training a network to play a game, or guiding a missile to the end of a level (as you shall see).

The first 4/5 of this document are defining functions to be used by the NEAT algorithm. Each one of these functions has a description at the beginning outlining its role in NEAT. The last part of this document contains the NEAT algorithm itself followed by the network training and the visualization.

