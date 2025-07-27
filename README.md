# AgPd-Nanoclusters-by-DRL

### Deep Reinforcenment Learning generation and optimization of Ag-Pd nanoclusters 

Please cite this paper:

    @article{Farooq_2025,
doi = {10.1088/1402-4896/adeccc},
url = {https://dx.doi.org/10.1088/1402-4896/adeccc},
year = {2025},
month = {jul},
publisher = {IOP Publishing},
volume = {100},
number = {7},
pages = {0759b7},
author = {Farooq, Muhammad Umar and Chen, Fuyi},
title = {Deep Reinforcement learning generation and optimization of AgPd nanoclusters},
journal = {Physica Scripta}

}
### How to Run the Code

1. **Set Up the Environment:**
   - Install the required Conda environment using the provided YAML file:
     ```bash
     conda env create -f AgPd.yml
     ```

2. **Configure the Nanocluster Composition:**
   - Edit `AgPd.py` to select the nanocluster composition.

   - **Monometallic Nanocluster:** For simulating a cluster of 5 atom silver (Ag) or palladium (Pd) atoms:
     ```python
     eleNames = ['Ag']
     eleNums = [5]
     ```
   - **Bimetallic Nanoclusters:** For simulating a bimetallic cluster of 10 silver (Ag) and 10 palladium (Pd) atoms:
     ```python
     eleNames = ['Ag', 'Cu']
     eleNums = [10, 10]
     ```

3. **Run the Simulation:**
   - Execute the script using Python. 
     ```bash
     python AgPd.py  
     ```

