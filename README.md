# Multi-Vehicle-Racing-Line-Optimization

Implementation of a IPOPT and Direct Collocation (DIRCOL) based Multi Vehicle Controller Optimization for an autonomous Formula 1 car. [[Paper]](https://github.com/NikhilCG26/Multi-Vehicle-Racing-Line-Optimization/blob/main/OCRL_Final_Paper.pdf)

**This repo supports**
* DIRCOL Trajectory Optimization for controller for Autonomous Racecars using IPOPT Solver
* Visualization using Julia Plot
* Visualization using MeshCat Libraries

## Introduction

In this repository, we propose a multi-vehicle racing line optimization strategy aimed at controlling two vehicles simultaneously in autonomous racing competitions is presented in this paper. The proposed control strategy is concerned with both cars completing the track in a given time competing for the optimal racing line. The optimization problem considers both the vehicle’s dynamics and upper and lower bounds for the states and vehicle controls. Furthermore, the approach allows the cars to safely race on a track while avoiding collision with each other in predefined trajectories. Simulations of both cars following the trajectories are shown using Meshcat. Although the control strategy allowed both cars to follow the given trajectories, there were minimal signs of the two vehicles battling for the optimal trajectory.
## Dependencies
Julia v1.6.7, Juptyer Notebook

## Installation
1. Install Julia. Download v1.6.7 from the Julia website. From here you can follow these platform specific instructions to get started.
2. Clone this repo and put it wherever you want.
3. Start a Julia REPL in your terminal using julia, or the location to the Julia binaries. If this doesn't work, make sure you followed the platform specific instructions.
4. Install the IJulia using the Julia package manager. In the REPL, enter the package manager using ], then enter add IJulia to add it to your system path.
5. In the REPL (hit backspace to exit these package manager), enter using IJulia
6. Launch the notebook using notebook() or jupyterlab()

## Trajectory Generation
The majority of the necessary code for the combined dynamics is located [Combined Dynamics](https://github.com/NikhilCG26/Multi-Vehicle-Racing-Line-Optimization/blob/main/Project_Combined_Dynamics.ipynb). 
For the double integrator model, reference [Double Integrator Model](https://github.com/NikhilCG26/Multi-Vehicle-Racing-Line-Optimization/blob/main/Project_Double_integrator_Dynamics.ipynb)
For Kinematics model alone, reference [Kinematics Model](https://github.com/NikhilCG26/Multi-Vehicle-Racing-Line-Optimization/blob/main/Project_base-Kinematics.ipynb). 
For Dynamics model alone, reference [Dynamics Model](https://github.com/NikhilCG26/Multi-Vehicle-Racing-Line-Optimization/blob/main/Project_base-Dynamics.ipynb). 
Run each jupyter notebook cell sequentially as described.

