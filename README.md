
# AgPd Nanoclusters by Deep Reinforcement Learning — DRL Framework for Ag-Pd Nanocluster Global Minimum Search (version 2.0).

### Deep Reinforcement Learning Generation and Optimization of Ag-Pd Nanoclusters

This is a modified and adapted version of the DRL framework from: 

**Exploring Nanocluster Potential Energy Surfaces via Deep Reinforcement Learning: Strategies for Global Minimum Search**<br>
Rajesh K. Raju <br>
 J. Phys. Chem. A 2024, 128, 9122−9134.
 The TRPO version of DRL framework is available at https://github.com/rajeshkochi444/clusgm_drl.
 
We thank the authors for making the code available on github.  

---

## Key Modifications

This framework replaced the original TRPO agent with PPO agent for faster wall-clock convergence, better sample efficiency, and correct on-policy exploration. 
We modified the code to work with AgPd nanoclusters.

---


### PPO hyperparameters

| Parameter | Default | Description |
|---|---|---|
| `batch_size` | `64` | Episodes collected before each policy update |
| `learning_rate` | `3e-4` | Adam learning rate |
| `optimization_steps` | `10` | Gradient passes per collected batch |
| `subsampling_fraction` | `0.25` | Mini-batch fraction per optimisation step |
| `likelihood_ratio_clipping` | `0.2` | PPO clip epsilon ε |
| `entropy_regularization` | `0.01` | Entropy bonus for exploration |
| `discount` | `0.99` | Reward discount factor γ |
| `timesteps` | `200` | Maximum steps per episode |

---


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

---
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

