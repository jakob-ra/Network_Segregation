# Network segregation
An agent-based model of segregation in social networks. A report that outlines the model and results can be found at: 

## Contents
* toy_model.py: A basic version of the model with a network visualization at every step. There are blue, red, and green agents. Choose parameters and run. Self-contained.
* fast_model.py: An updated version of the model where agent's utility gains from all possible links are pre-calculated. Every step,  all agents get to revise one link. This speeds up computation dramatically (which is required for sensitivity analysis and validation on large schools). The model uses agent characteristics (students' sex, race, and grade) from the ADD Health data set. This data has to be downloaded to the working directory from https://drive.google.com/open?id=1CjBQYX9WXxwgdwVkgpXEOPQyrvQGapJW (90 MB).
* SA_superspeed.py: Uncertainty analysis and sensitivity analysis (one at a time and global/Sobol).
* validation.py: Finds parameter values that generates networks with the same characteristics as the observed friendship network via grid search.
