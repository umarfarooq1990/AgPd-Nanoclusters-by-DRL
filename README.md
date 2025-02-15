# AgPd Nanoclusters by DRL

## DRL Framework for Nanocluster Global Minimum Search

We have developed a Deep Reinforcement Learning (DRL) framework for exploring nanoclusters, efficiently identifying ground state and low-energy configurations.


## How to Run the Code

### Set Up the Environment:

Install the required Conda environment using the provided YAML file:

conda env create -f env_drl.yml

### Configure the Nanocluster Composition:

Edit gym_trpo_single.py to select the desired nanocluster composition.

### For simulating the monometallic nanocluster of 5 Silver (Ag) atoms:

eleNames = ['Ag']

eleNums = [5]

### For simulating the bimetallic nanocluster:

eleNames = ['Ag', 'Pd']

eleNums = [2, 3]

## Run the Simulation:

Execute the script using Python.

python gym_trpo_single.py

