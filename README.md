# ABM_political_election

## Model definition
With this political election model we studied different types of voting systems with different politcal party positions. To study this we used an agent based modelling approach. In this model the agents are the polical parties and the voters.

## Experiment setup
Different types of voting systems are tested under various party setups. The party positions that we used for our research can be seen in 'running the model'. We studied three different voting systems on these party setups, namely the plurality voting system, the approval voting system and the instant runoff voting system.

## Statistical analysis
The stastical analysis is done with the Kolmogorov-Smirnov test. The results of these tests can be seen in the file stats test.ipynb. The results that were used for these stastical tests can be found in the .txt files.

## Sensitivity analysis

For sensitivity analysis you need the model definition script and several packages like MESA, NetworkX, SAlib etc. The script contains the creation of the problem and the model output function, the Sobol analysis and the scripts for plotting the results

## Running the model
To run the model simply run the cells in the notebook, the most important cell is labelled "Test model with graphical analyses", this cell can be used to run the model with specific party placements and get useful information about the result of the simulation. Some instructions on how to use it:

Party positions:
Equal spacing square = [(50, 50),(50, 150),(150, 50),(150,150)]
Center squeeze = [(75,100),(100,100),(125,100)]
spoiler effect = [(100, 29.29),(75, 166.14),(100, 170.71),(125,166.14)]
Or something else (can be anything, really)

Change initial_party_pos to the positions you want, or leave empty for random positions (amount = initial_parties parameter)
If animation is False only the last graph will be plotted

The parameters of the model can be changed in the cell labelled as "parameters"
