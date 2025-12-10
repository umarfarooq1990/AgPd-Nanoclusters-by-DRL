
# AgPd Nanoclusters by Deep Reinforcement Learning

### Deep Reinforcement Learning Generation and Optimization of Ag-Pd Nanoclusters

For detailed insights, please refer to the paper:  
[Deep Reinforcement Learning Generation and Optimization of Ag-Pd Nanoclusters](https://github.com/user-attachments/files/21455604/Deep.Reinforcement.Learning.generation.and.optimization.of.AgPd.nanoclusters.pdf)

### How to Run the Code

#### 1. **Set Up the Environment:**
   - First, install the required Conda environment by using the provided YAML configuration file:
     ```bash
     conda env create -f AgPd.yml
     ```

#### 2. **Configure the Nanocluster Composition:**
   - Modify the `AgPd.py` script to select the desired nanocluster composition.

   - **Monometallic Nanocluster:** To simulate a cluster of 5 silver (Ag) or palladium (Pd) atoms, use the following configuration:
     ```python
     eleNames = ['Ag']
     eleNums = [5]
     ```
     Or, for palladium (Pd):
     ```python
     eleNames = ['Pd']
     eleNums = [5]
     ```

   - **Bimetallic Nanoclusters:** To simulate a bimetallic cluster with 10 silver (Ag) and 10 palladium (Pd) atoms, configure the script as follows:
     ```python
     eleNames = ['Ag', 'Pd']
     eleNums = [10, 10]
     ```

#### 3. **Run the Simulation:**
   - Once the nanocluster composition is configured, execute the script using Python:
     ```bash
     python AgPd.py
     ```

### Note
Any nanocluster configuration can be simulated by changing the `eleNames` and `eleNums` parameters in the script. This includes **monometallic**, **bimetallic**, **trimetallic**, **quaternary**, and **quinary** alloy compositions. Simply specify the desired elements and their respective atomic counts in the `eleNames` and `eleNums` lists to customize the simulation.

### Citation

Please cite the following paper if you use this code in your research:

```bibtex
{
@article{Farooq_2025,
    title = {Deep Reinforcement Learning Generation and Optimization of AgPd Nanoclusters},
    author = {Farooq, Muhammad Umar and Chen, Fuyi},
    doi = {10.1088/1402-4896/adeccc},
    journal = {Physica Scripta},
    year = {2025},
    publisher = {IOP Publishing}
}
```

### Open Source Code

This project is open-source, and we encourage you to use and contribute to it. The code is available under the [MIT License](LICENSE). Feel free to fork, modify, and distribute the code as needed. We welcome contributions and feedback from the community to improve the functionality and performance of the model.
