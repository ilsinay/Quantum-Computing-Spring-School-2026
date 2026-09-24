# Quantum Computing Spring School 2026

Tutorial notebooks for the computing stream of the SAQUTI Quantum Technologies
School: four hands-on sessions that take you from your first lines of Python to
simulating quantum systems with [Qiskit](https://www.ibm.com/quantum/qiskit).

No prior programming experience is assumed. Everything runs on your own laptop
using classical simulators, so you don't need an IBM Quantum account.

## Sessions

| # | Session | Material |
|---|---|---|
| 1 | **Introduction to Python for Quantum Computing**: variables, control flow, data structures, functions, packages and environments, NumPy, SciPy and Matplotlib | [notebook](session-1-python-intro/01_intro_python_for_quantum_computing.ipynb) · [PDF](session-1-python-intro/01_intro_python_for_quantum_computing.pdf) |
| 2 | **Quantum States, Circuits & Measurement**: qubits, unitaries and measurement built by hand in NumPy, then the same ideas in Qiskit | coming soon |
| 3 | **Quantum Algorithms**: oracles and phase kickback, Deutsch–Jozsa, and Grover's search | coming soon |
| 4 | **Quantum Simulation of Hamiltonians**: Trotter, Suzuki and QDrift product formulas, applied to the transverse-field Ising chain | coming soon |

Each session is a Jupyter notebook you work through live. Exercises are
followed by a solution cell, so try each one before running the solution.
The PDF has the same content as printable notes.

## Before the school: set up your laptop

Please do this **at least a few days before the school starts**.

1. Follow the [pre-school setup guide](setup/pre_school_setup_guide.pdf). It
   walks you through installing Anaconda, creating the `saqutischool`
   environment and installing Qiskit on Windows, macOS or Linux.
2. Download this repository (see below), start JupyterLab from your
   `saqutischool` environment, and open
   [`setup/00_environment_check.ipynb`](setup/00_environment_check.ipynb).
3. Run all cells (**Run → Run All Cells**). If you see a circuit diagram and a
   histogram with two bars of about equal height, you're ready.

Having trouble? Get in touch with the organisers **before** you arrive, so
setup problems don't eat into session time.

## Getting the material

With git:

```bash
git clone https://github.com/ilsinay/Quantum-Computing-Spring-School-2026.git
cd Quantum-Computing-Spring-School-2026
```

Without git, use **Code → Download ZIP** on the
[repository page](https://github.com/ilsinay/Quantum-Computing-Spring-School-2026)
and unzip it.

New sessions will be added here before the school. If you cloned with git,
`git pull` fetches them. If you downloaded the ZIP, download it again.

## Repository layout

```
setup/                   Setup guide (PDF) and the environment check notebook
session-1-python-intro/  Session 1 notebook and PDF notes
```

## Licence

[MIT](LICENSE)
