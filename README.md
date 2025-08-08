Overview
This repository contains a clear, educational implementation of the Coursera “Building Neural Networks (one hidden layer)” assignment. It is intended for students who want a reproducible reference implementation and for instructors who want straightforward notebooks for grading. Everything is written in plain Python + NumPy (no high-level frameworks), with numbered notebook cells and helper scripts to reproduce experiments and plots.

Features
Step-by-step Jupyter notebooks (cells numbered for easy grading)

Pure NumPy implementations of forward/backward propagation, initialization, and gradient descent

Visualization utilities for decision boundaries and loss/accuracy curves

Unit tests to validate core functions

Sample synthetic datasets used in the assignment

Scripts to run training end-to-end and reproduce figures from the assignment

Repository structure
bash
Copy
Edit
.
├── notebooks/
│   ├── 01_building_nn.ipynb      # Main assignment notebook (cell numbers included)
│   └── 02_experiments.ipynb      # Additional experiments & ablations
├── src/
│   ├── nn/
│   │   ├── layers.py             # linear, activations, forward/backward
│   │   ├── init.py               # parameter initialization
│   │   ├── model.py              # model training & predict
│   │   └── utils.py              # helper functions (loss, accuracy, etc.)
│   └── data/
│       └── generate.py           # small synthetic datasets
├── tests/
│   ├── test_layers.py
│   └── test_model.py
├── examples/
│   └── run_experiment.py         # script to reproduce decision boundary plots
├── requirements.txt
├── .python-version                # recommended python (optional)
└── README.md
Requirements
Python 3.8+ (tested on 3.8–3.11)

Packages listed in requirements.txt (NumPy, matplotlib, pytest, jupyter, notebook, etc.)

Install:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
