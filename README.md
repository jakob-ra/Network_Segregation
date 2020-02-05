# Network segregation
An agent-based model of segregation in social networks. A report that outlines the model and results can be found at: 

## Contents
* toy_model.py: A basic version of the model with a network visualization at every step. There are blue, red, and green agents. Choose parameters and run. Self-contained.
* model.py: An updated version of the model where agent's utility gains from all possible links are pre-calculated. Every step,  all agents get to revise one link. This speeds up computation dramatically (which is required for sensitivity analysis and validation on large schools). The model uses agent characteristics (students' sex, race, and grade) from the ADD Health data set.
* SA.ipynb: Uncertainty analysis and sensitivity analysis (one at a time and global/Sobol).
* validation.ipynb: Finds parameter values that generates networks with the same characteristics as the observed friendship network. Plots comparisons between generated and observed networks.
