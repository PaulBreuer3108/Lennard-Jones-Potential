# Lennard-Jones Potential Simulation

This repository contains a Python implementation for simulating the Lennard-Jones potential, which is used to model the interaction between pairs of neutral atoms or molecules. The simulation includes energy minimization of nanoclusters using the conjugate gradient method.

## Authors
- Paul Breuer

## Table of Contents
1. [Introduction](#introduction)
2. [Requirements](#requirements)
3. [Usage](#usage)
4. [Code Structure](#code-structure)
5. [Results](#results)
6. [References](#references)

## Introduction
The Lennard-Jones potential is a mathematical model that approximates the interaction between a pair of neutral atoms or molecules. This project focuses on minimizing the potential energy of nanoclusters using the conjugate gradient method. The simulation is performed for clusters ranging from 2 to 25 atoms.

## Requirements
To run the code, you need the following Python packages:
- `numpy`
- `matplotlib`
- `scipy`
- `ase` (Atomic Simulation Environment)

You can install the required packages using pip:
```bash
pip install numpy matplotlib scipy ase

### Usage
1. Clone the repository:
  ```bash
  git clone https://github.com/yourusername/lennard-jones-simulation.git
  cd lennard-jones-simulation
  ```

2. Run the jupyter Notebook:
  ```bash
  jupyter notebook Jupyter.ipynb
  ```

3. Execute the cells in the notebook to perform the simulation and visualize the results.

# Energy Minimization Simulation

This repository contains a simulation for energy minimization using the conjugate gradient method. The code calculates the minimum potential energy of atomic clusters and compares the results with macroscopic scaling estimates.

## Code Structure

The code is structured as follows:

1. **Imports**: Necessary libraries are imported.

2. **Simulation Parameters**:  
   Parameters such as `delta`, `M`, `dimensions`, `LStol`, `ECtol`, `MaxLSSteps`, and `MaxCGSteps` are defined.

3. **Global Variables**:  
   Variables like `Time_calculating_forces` and `goal_energy` are initialized.

4. **Functions**:
   - `initialize_positions`: Initializes the positions of atoms.
   - `find_distance`: Calculates the distance between two atoms.
   - `calculate_potential_energy`: Computes the potential energy of the system.
   - `calculate_forces`: Calculates the forces acting on each atom.
   - `calculate_energy_and_forces`: Combines energy and force calculations.
   - `interpolation`: Performs quadratic interpolation.
   - `line_search`: Performs line search for energy minimization.
   - `conjugate_gradient_minimization`: Minimizes the energy using the conjugate gradient method.
   - `perform_the_minimization_for_different_starting_positions`: Runs the minimization for different starting positions.
   - `plot_results_task2`: Plots the results for Task 2.
   - `U_macro`: Function for macroscopic scaling estimate.

5. **Main**:  
   Executes the simulation and prints the total time elapsed.

---

## Results

The simulation results include:

1. **Minimum Potential Energy**:  
   The minimum potential energy is calculated for clusters of different sizes.

2. **Convergence Steps**:  
   The number of conjugate gradient steps required for convergence is reported.

3. **Plots**:  
   - The potential energy at each iteration for different cluster sizes is plotted.
   - A comparison of the simulated potential energy with the macroscopic scaling estimate.

---
