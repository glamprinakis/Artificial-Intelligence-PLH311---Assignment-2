Artificial Intelligence PLH311 - 2nd Programming Assignment

This repository contains the solution for the second programming assignment of the Artificial Intelligence (PLH311) course. The assignment focuses on developing a search agent for the game TUC-CHESS, a custom chess variant where capturing certain positions awards points to the player.

Summary
The main goal of this project was to implement and compare three different AI algorithms for optimal move selection in TUC-CHESS:

Minimax
Alpha-Beta Pruning
Monte Carlo Tree Search (MCTS)
Implementation Highlights

Game Representation:
The game's state and possible moves are modeled using custom Java classes (Move, MoveComparator, Agent).
Minimax Algorithm:
Classic adversarial search, implemented with move ordering for better performance.
Alpha-Beta Pruning:
Optimizes Minimax by pruning branches that cannot affect the outcome, using evaluation and cutoff functions to reduce unnecessary search.
Monte Carlo Tree Search (MCTS):
Simulates multiple random play-outs from each position and statistically determines the best move, following the stages of selection, expansion, simulation, and backpropagation.
