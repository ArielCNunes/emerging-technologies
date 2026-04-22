# Emerging Technologies

Assessments focused on quantum computing, exploring the [Deutsch–Jozsa algorithm](https://en.wikipedia.org/wiki/Deutsch%E2%80%93Jozsa_algorithm) through a series of progressive problems implemented in [Python](https://www.python.org/) and [Qiskit](https://www.ibm.com/quantum/qiskit).

## Contents

The notebook `problems.ipynb` will cover five problems:

| Problem | Title | Description |
|---------|-------|-------------|
| 1 | Generating Random Boolean Functions | Implements `random_constant_balanced()`, a test data generator that returns a randomly chosen constant or balanced Boolean function over four inputs |
| 2 | Classical Testing for Function Type | Implements a classical algorithm to determine whether a function is constant or balanced, with an optimised version using the [pigeonhole principle](https://en.wikipedia.org/wiki/Pigeonhole_principle) (worst case: 9 function calls) |
| 3 | Quantum Oracles | Builds the four single-input quantum oracles (f₀–f₃) using X and CX gates, verifies their circuit diagrams, and simulates their behaviour on all input states |
| 4 | [Deutsch's Algorithm](https://en.wikipedia.org/wiki/Deutsch%E2%80%93Jozsa_algorithm#Deutsch's_algorithm) with Qiskit | Implements Deutsch's algorithm in Qiskit using the Problem 3 oracles, explains phase kickback, and verifies constant vs balanced classification with one oracle query |
| 5 | Scaling to the Deutsch–Jozsa Algorithm | Extends to a 4-input Deutsch-Jozsa implementation by building a 5-qubit oracle with MCX gates, constructing the full circuit, and validating outcomes on simulation |

## Requirements

This notebook was tested on **Python 3.12.1**.

Install dependencies with:

```bash
pip install -r requirements.txt
```

Key packages:

- [`qiskit[visualization]`](https://docs.quantum.ibm.com/) — quantum circuit construction and transpilation
- [`qiskit-aer`](https://qiskit.github.io/qiskit-aer/) - local quantum circuit simulator
- [`jupyterlab`](https://jupyterlab.readthedocs.io/) / [`notebook`](https://jupyter-notebook.readthedocs.io/) — notebook environment
- [`matplotlib`](https://matplotlib.org/) — circuit diagram rendering

## Running the Notebook

**With JupyterLab:**

```bash
jupyter lab problems.ipynb
```

**With Jupyter Notebook:**

```bash
jupyter notebook problems.ipynb
```

**With VS Code:**

Open `problems.ipynb` in VS Code with the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) installed, select a Python kernel, and run all cells with **Run All**.

Cells must be run in order from top to bottom, as later cells depend on functions defined in earlier ones.
