---
title: FitSNAP
---

# FitSNAP Tutorial

## Workflow for each notebook:
1. Connect their laptop to the network

2. Click on first link, click on cell [1], hit Shift+Enter

3. Confirm that the top-left symbol is spinning around

4. Repeat for links 2 and 3

5. In each case, the first cell will finish running in ~15 minutes.

6. After that, things are more instantaneous

## Tutorial Notebooks

The following notebooks are also available on the FitSNAP repo [here](https://github.com/jmgoff/FitSNAP-1/tree/update_tutorials)

+ **Simple linear fit and general FitSNAP tutorial:**

Contains simple ACE & SNAP fits for Ta and some general info about ACE parameters

General Fitsnap in/out : settings, .yace potential file, .mod file to run lammps (with ZBL )

RMSE printed for ACE and SNAP allow you to compare accuracy between the two model types

https://colab.research.google.com/github/jmgoff/FitSNAP-1/blob/update_tutorials/tutorial.ipynb 

+ **Multi-element fits & end-to-end lammps MD tutorial:**

Contains more detailed info about linear ACE fits for Ta and InP. 

Fit both examples, but use generated Ta potential to run MD in lammps. Allows students to view Temp vs Timestep through matplotlib. 

https://colab.research.google.com/github/jmgoff/FitSNAP-1/blob/update_tutorials/tutorial_ace_inp_and_lammps_md.ipynb

+ **Hyperparameter sweeps, optimization and FitSNAP Genetic Algorithm Tutorial:**

Contains ridge alpha penalty sweeps

Ta models with sweeps over descriptor set sizes

Model comparisons with different regression/Solver types ( SVD, Ridge, ARD )

Contains a small ~ 60s long genetic algorithm sweep to optimize group weights.

https://colab.research.google.com/github/jmgoff/FitSNAP-1/blob/update_tutorials/tutorial_ace_solvers_and_optimization.ipynb



