# Stochastic-processes
University assessments related to stochastic processes, random walks, Markov chains, and many more simulations.

# Simulation and Analysis of the Simple Random Walk (SRW)

This repository contains the implementation and visual analysis of a discrete-time **Simple Random Walk (SRW)**, developed in Python using `NumPy` and `Matplotlib`. The main objective is to model stochastic trajectories and empirically verify the fundamental mathematical properties of the process.

## Project Features

* **Efficient Vectorization:** The core function `simular_PAS` is designed to avoid explicit `for` loops. It leverages multidimensional arrays and NumPy axis operations (`np.random.choice`, `np.cumsum`) to generate thousands of trajectories in a fast and computationally efficient manner.
* **Parametric Flexibility:** It allows adjusting the probability of success (p), the number of steps (n), and the number of independent simulations (reps), modeling both symmetric walks and those with a drift.

## Included visualizations

The notebook reproduces the following theoretical scenarios:

1. **Drift Exploration (Visualization 1):** Comparison of individual trajectories under different probabilities (p=0.5, 0.6, 0.4), showing how the parameter affects the drift of the walk.
2. **Theoretical Bounds and Chebyshev's Inequality (Visualization 2):** Multiple trajectories are plotted, superimposing the **theoretical mean** and the **dispersion bands** of 1 and 2 standard deviations. This allows for visual verification that most paths remain within the expected probabilistic limits.
3. **Law of Large Numbers (Visualization 3):** Convergence analysis comparing the theoretical mean with the empirical mean. It demonstrates how, by averaging an increasing number of trajectories (from 5 to 1000), the result converges towards the theoretical mean function.

## Technologies used
* Python 3
* NumPy (Random array generation and matrix computations)
* Matplotlib (Time series visualization and confidence areas)
