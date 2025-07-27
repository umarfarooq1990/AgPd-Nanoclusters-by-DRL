# AgPd-Nanoclusters-by-DRL

### Deep Reinforcenment Learning generation and optimization of Ag-Pd nanoclusters 

[Deep Reinforcement Learning generation and optimization of AgPd nanoclusters.pdf](https://github.com/user-attachments/files/21455604/Deep.Reinforcement.Learning.generation.and.optimization.of.AgPd.nanoclusters.pdf)

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
     eleNames = ['Ag', 'Pd']
     eleNums = [10, 10]
     ```

3. **Run the Simulation:**
   - Execute the script using Python. 
     ```bash
     python AgPd.py  

Please cite this paper:

    @article{Farooq_2025,
    title = {Deep Reinforcement learning generation and optimization of AgPd nanoclusters},
    author = {Farooq, Muhammad Umar and Chen, Fuyi},
    doi = {10.1088/1402-4896/adeccc},
    journal = {Physica Scripta}
    year = {2025},
    publisher = {IOP Publishing},
    
