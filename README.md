# Endogenous Feedback in Coevolutionary Games Reshapes the Stability of Cooperation

This repository contains the code associated with the paper:

**Federico Maria Quetti, Andrea Civilini, Giacomo Frigerio, Silvia Figini, Giacomo Livan, Vito Latora (2025).**  
**"Endogenous Feedback in Coevolutionary Games Reshapes the Stability of Cooperation"**  
arXiv: https://arxiv.org/abs/2506.20603

This work studies how endogenous coevolution between population behavior and the payoff structure of an evolutionary game can generate *chimera games*: stable cooperation levels that do not correspond to any equilibrium of the associated static (i.e. no-feedback) game.

The repository contains:

- A numerical analysis of the replicator dynamics with endogenous feedback (`NumericalAnalysis.ipynb`)
- Monte Carlo simulations in well-mixed populations (`Simulations.py`)
- Main paper plots showing the evolution of cooperation over time and the trajectory of the game in the dilemma-strength square (`Paper_plots.ipynb`)
- Detailed analysis of the delayed-feedback case, including figures used in the paper (`delay_analysis.ipynb`)

---

## Repository Contents

### `NumericalAnalysis.ipynb`

This notebook performs a numerical investigation of the fixed points of the replicator equation with feedback. It includes:

- Evaluation of the fixed-point equation on a grid of (Dg, Dr) values  
- Computation of equilibrium points in the interval [0, 1]  
- Stability analysis based on the derivative  
- Detection of regions with 0, 1, or 2 interior equilibria  
- Phase-line diagrams illustrating representative dynamical scenarios  
- Computation of the equilibrium game resulting from feedback  
- Identification of "chimera games", i.e., stable equilibria that are not admissible under classical static evolutionary game theory

### `Simulations.py`

This script implements Monte Carlo simulations for a finite, well-mixed population:

- Population size N = 2500  
- Two strategies: C and D  
- Payoff matrix updated at each step using the current cooperation level  
- Interactions with k = 4 random partners  
- Strategy updates through the Fermi imitation rule  
- Simulations performed for 20 (Dr, Dg) parameter pairs across four social dilemma classes (PD, HG, SD, SH)  
- Multiple initial cooperation levels (0.1, 0.3, 0.5, 0.7, 0.9)  
- Produces a 4-by-5 grid figure showing the evolution of cooperation and the instantaneous game played

### `Paper_plots.ipynb`

This notebook generates the main paper plots. It includes:

- Evolution of cooperation over time  
- Reconstruction of the instantaneous game played during the dynamics  
- Visualization of the game trajectory in the dilemma-strength square (Dg, Dr)  
- Figures showing how endogenous feedback moves the system across different social dilemma classes  

### `delay_analysis.ipynb`

This notebook contains the detailed analysis of the delayed-feedback case. It includes:

- Implementation of the delayed replicator dynamics  
- Computation of equilibrium cooperation levels  
- Linear stability analysis around delayed-feedback equilibria  
- Calculation of the critical delay for the onset of oscillations  
- Numerical simulations for different delay values  
- Figures used in the paper for the delayed-feedback analysis  

## Citation

If you use this code, please cite:

Quetti, F. M., Civilini, A., Frigerio, G., Figini, S., Livan, G., and Latora, V. (2025).  
"Endogenous Feedback in Coevolutionary Games Reshapes the Stability of Cooperation"  
arXiv: 2506.20603. https://arxiv.org/abs/2506.20603
