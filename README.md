# Emerging Technologies

Assessments focused on quantum computing, exploring the Deutsch–Jozsa algorithm through a series of progressive problems implemented in Python and Qiskit.

## Contents

The notebook `problems.ipynb` will cover five problems:

| Problem | Title | Description |
|---------|-------|-------------|
| 1 | Generating Random Boolean Functions | Implements `random_constant_balanced()`, a test data generator that returns a randomly chosen constant or balanced Boolean function over four inputs |
| 2 | Classical Testing for Function Type | Implements a classical algorithm to determine whether a function is constant or balanced, with an optimised version using the pigeonhole principle (worst case: 9 function calls) |
| 3 | Quantum Oracles | Builds the four single-input quantum oracles (f₀–f₃) using X and CX gates, verifies their circuit diagrams, and simulates their behaviour on all input states |
| 4 | Deutsch's Algorithm with Qiskit | N/A |
| 5 | Scaling to the Deutsch–Jozsa Algorithm | N/A |

## Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

Key packages:

- `qiskit[visualization]` — quantum circuit construction and transpilation
- `qiskit-aer` — local quantum circuit simulator
- `jupyterlab` / `notebook` — notebook environment
- `matplotlib` — circuit diagram rendering

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

> Cells must be run in order from top to bottom, as later cells depend on functions defined in earlier ones.
