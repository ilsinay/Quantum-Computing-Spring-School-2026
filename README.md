# Quantum Computing Spring School 2026

Tutorial notebooks and notes for the
[Quantum Computing Spring School 2026](https://afriqa.ukzn.ac.za/event/quantum-computing-spring-school-2026/),
hosted by the African Quantum Alliance (AfriQA) and the University of
KwaZulu-Natal, 24–26 September 2026.

## About the school

The spring school is aimed at Honours, Master's and Doctoral students, and
covers:

- Basic quantum algorithms
- Variational quantum algorithms
- Simulation of quantum systems
- Quantum machine learning

Lecturers: Ian David (UKZN), Thomas Konrad (UKZN), Matt Lourens (Stellenbosch
University), Shivani Pillay (UKZN) and Ilya Sinayskiy (UKZN).

For the programme, venue and contact details, see the
[school's event page](https://afriqa.ukzn.ac.za/event/quantum-computing-spring-school-2026/).

## Tutorials

The tutorials are Jupyter notebooks you work through on your own laptop. All
code runs on classical simulators, so you don't need access to quantum
hardware or an IBM Quantum account. Exercises are followed by a solution cell,
so try each one before running the solution.

Sessions are numbered in the order of the school programme, so a few numbers
are not used by a tutorial yet.

| Session | Programme slot | Tutorial | Material |
|---|---|---|---|
| 1 | Thu 24 Sep · Lecture 1 | **Basic Quantum Algorithms** (lecture slides) | [slides](session-1-lecture-basic-quantum-algorithms/QCworkshop24.Sept.pdf) |
| 2 | Thu 24 Sep, 14:00 · Python for Quantum Computing | **Introduction to Python for Quantum Computing**: variables, control flow, data structures, functions, packages and environments, NumPy, SciPy and Matplotlib. No prior programming experience assumed. | [notebook](session-2-python-intro/02_intro_python_for_quantum_computing.ipynb) · [PDF notes](session-2-python-intro/02_intro_python_for_quantum_computing.pdf) |
| 4 | Thu 24 Sep, 20:00 · Qiskit Lab I: Basics of Quantum Computing | **Quantum States, Circuits & Measurement**: qubit states, unitaries, circuits and measurement built by hand in NumPy and SciPy, then the same ideas in Qiskit with `QuantumCircuit`, `Statevector`, samplers, estimators and the Aer simulator. | [notebook](session-4-quantum-computing-qiskit/04_intro_quantum_computing_qiskit.ipynb) · [PDF notes](session-4-quantum-computing-qiskit/04_intro_quantum_computing_qiskit.pdf) |
| 5 | Fri 25 Sep, 09:00 · Qiskit Lab II: Basics of Quantum Computing | **Quantum Algorithms**: oracles and phase kickback, the Deutsch–Jozsa algorithm, and Grover's search, including how many iterations Grover needs and why. | [notebook](session-5-quantum-algorithms-qiskit/05_quantum_algorithms_qiskit.ipynb) · [PDF notes](session-5-quantum-algorithms-qiskit/05_quantum_algorithms_qiskit.pdf) |
| 8 | Fri 25 Sep, 16:00 · Qiskit Lab III: VQE | **Variational Quantum Eigensolver (VQE)** | [notebook](session-8-vqe/vqe_tutorial_student.ipynb) |
| 9 | Fri 25 Sep, 20:00 · Qiskit Lab IV: QAOA | **QAOA for MaxCut** | [notebook](session-9-QAOA/09_QAOA_MaxCut.ipynb) |
| 13 | Sat 26 Sep, 16:00 · QSim laboratory | **Quantum Simulation of Hamiltonians**: why Hamiltonian simulation matters, first- and second-order Trotter–Suzuki product formulas and QDrift, compared on the transverse-field Ising chain. | [notebook](session-13-quantum-simulation-qiskit/13_quantum_simulation_qiskit.ipynb) · [PDF notes](session-13-quantum-simulation-qiskit/13_quantum_simulation_qiskit.pdf) |

More tutorials will be added to this repository as the school goes on.

## Setting up your laptop

1. Follow the [setup guide](setup/pre_school_setup_guide.pdf). It walks you
   through installing Anaconda, creating the `saqutischool` environment and
   installing [Qiskit](https://www.ibm.com/quantum/qiskit) on Windows, macOS
   or Linux.
2. Download this repository (see below), start JupyterLab from your
   `saqutischool` environment, and open
   [`setup/00_environment_check.ipynb`](setup/00_environment_check.ipynb).
3. Run all cells (**Run → Run All Cells**). If you see a circuit diagram and a
   histogram with two bars of about equal height, you're ready.

If something doesn't work, ask one of the tutors.

## Getting the material

With git:

```bash
git clone https://github.com/ilsinay/Quantum-Computing-Spring-School-2026.git
cd Quantum-Computing-Spring-School-2026
```

To fetch tutorials added later, run `git pull` inside that folder.

Without git, use **Code → Download ZIP** on the
[repository page](https://github.com/ilsinay/Quantum-Computing-Spring-School-2026)
and unzip it. Download it again to get new tutorials.

## Repository layout

```
setup/                                      Setup guide (PDF) and the environment check notebook
session-1-lecture-basic-quantum-algorithms/ Session 1: Lecture 1 slides
session-2-python-intro/                     Session 2: Python for Quantum Computing
session-4-quantum-computing-qiskit/         Session 4: Qiskit Lab I
session-5-quantum-algorithms-qiskit/        Session 5: Qiskit Lab II
session-8-vqe/                              Session 8: Qiskit Lab III (VQE)
session-9-QAOA/                             Session 9: Qiskit Lab IV (QAOA)
session-13-quantum-simulation-qiskit/       Session 13: QSim laboratory
```

## Licence

[MIT](LICENSE)
