# Learning-based Control — Course Notebooks

This repository contains the Jupyter notebooks from the coding units of the MOOC
[**RWTHx: Learning-based Control**](https://www.edx.org/learn/computer-science/rwth-aachen-university-learning-based-control).

All notebooks build on the cart pole as a running example:

| Notebook | Topic |
| --- | --- |
| `notebooks/week2_lqr-sol.ipynb` | LQR for stabilizing the upper equilibrium of the cart pole |
| `notebooks/week3_dynamics_learning_discrete-sol.ipynb` | Learning a discrete-time dynamics model with PyTorch |
| `notebooks/week4_bo-sol.ipynb` | Tuning an LQR with Bayesian optimization |
| `notebooks/week5_REINFORCE-sol.ipynb` | REINFORCE on the Gymnasium CartPole environment |
| `notebooks/week6_mpc-sol.ipynb` | Cart pole swing-up with model predictive control |

## Setup

The notebooks were developed and tested with **Python 3.11**.

### 1. Clone the repository

```bash
git clone https://github.com/Data-Science-in-Mechanical-Engineering/mooc_lbc.git
cd mooc_lbc
```

### 2. Create a virtual environment

Using `venv`:

```bash
python3.11 -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
```

Or using `conda`:

```bash
conda create -n mooc_lbc python=3.11
conda activate mooc_lbc
```

### 3. Install the dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

The versions in `requirements.txt` are pinned to the ones the notebooks were
developed and tested with. If you prefer newer versions, drop the pins — but note
that `torch`, `botorch` and `gpytorch` change their APIs fairly often.

### 4. Start Jupyter

```bash
jupyter lab
```

Then open any notebook in the `notebooks/` folder and run the cells from top to
bottom. Each notebook is self-contained — there is nothing else to download.
