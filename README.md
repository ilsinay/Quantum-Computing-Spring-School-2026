# Quantum Computing Spring School 2026

Lecture slides, notes and tutorial notebooks from the
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

## Sessions

Folders are numbered by session, in the order of the school programme. Lectures
come with slides or notes; laboratories are Jupyter notebooks you work through
on your own laptop. All code runs on classical simulators, so you don't need
access to quantum hardware or an IBM Quantum account.

| # | When | Programme | Material |
|---|---|---|---|
| 1 | Thu 24 Sep | Lecture 1: Basic Quantum Algorithms (Deutsch, Deutsch–Jozsa, Grover) | [slides](session-01-basic-quantum-algorithms/QCworkshop24.Sept.pdf) |
| 2 | Thu 24 Sep, 14:00 | Python for Quantum Computing | [notebook](session-02-python-for-quantum-computing/02_intro_python_for_quantum_computing.ipynb) · [PDF notes](session-02-python-for-quantum-computing/02_intro_python_for_quantum_computing.pdf) |
| 3 | Thu 24 Sep, 16:00 | Quantum Computing Essentials | not in this repository |
| 4 | Thu 24 Sep, 20:00 | Qiskit Lab I: Basics of Quantum Computing (states, circuits and measurement) | [notebook](session-04-qiskit-lab-1/04_intro_quantum_computing_qiskit.ipynb) · [PDF notes](session-04-qiskit-lab-1/04_intro_quantum_computing_qiskit.pdf) |
| 5 | Fri 25 Sep, 09:00 | Qiskit Lab II: Basics of Quantum Computing (oracles, Deutsch–Jozsa, Grover) | [notebook](session-05-qiskit-lab-2/05_quantum_algorithms_qiskit.ipynb) · [PDF notes](session-05-qiskit-lab-2/05_quantum_algorithms_qiskit.pdf) |
| 6–7 | Fri 25 Sep, 11:00 and 14:00 | Variational Quantum Algorithms I and II | [slides](session-06-07-variational-quantum-algorithms/VQA.pdf) · [handwritten notes](session-06-07-variational-quantum-algorithms/25%20Sep%202026%20Handwritten%20notes%20by%20Dr%20Matt%20Lourens.pdf) |
| 8 | Fri 25 Sep, 16:00 | Qiskit Lab III: VQE | [student notebook](session-08-qiskit-lab-3-vqe/vqe_tutorial_student.ipynb) · [solutions](session-08-qiskit-lab-3-vqe/vqe_tutorial_solution.ipynb) |
| 9 | Fri 25 Sep, 20:00 | Qiskit Lab IV: QAOA (MaxCut) | [notebook](session-09-qiskit-lab-4-qaoa/05_QAOA_MaxCut.ipynb) · [reference paper](session-09-qiskit-lab-4-qaoa/fphy-02-00005.pdf) |
| 10 | Sat 26 Sep, 09:00 | NISQ QML: QSVM, QNN, QCNN | [slides](session-10-nisq-qml/Spring%20School%202026%20-%20NISQ%20QML.pdf) |
| 11 | Sat 26 Sep, 11:00 | Quantum simulation | [slides](session-11-quantum-simulation/Introduction%20to%20quantum%20simulation.pdf) |
| 12 | Sat 26 Sep, 14:00 | QML laboratory | [QSVM (iris)](session-12-qml-laboratory/qsvm_iris_qiskit-2.ipynb) · [QNN (penguins)](session-12-qml-laboratory/qnn_penguins_qiskit.ipynb) · [QCNN (pulsars)](session-12-qml-laboratory/qcnn_pulsars_qiskit.ipynb) |
| 13 | Sat 26 Sep, 16:00 | QSim laboratory (Trotter, Suzuki and QDrift) | [notebook](session-13-qsim-laboratory/13_quantum_simulation_qiskit.ipynb) · [PDF notes](session-13-qsim-laboratory/13_quantum_simulation_qiskit.pdf) |

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

Some laboratories use packages beyond the setup guide:

- **Session 9 (QAOA)** needs `networkx`: run `pip install networkx` in your
  activated `saqutischool` environment.
- **Session 12 (QML)** notebooks install what they need (such as
  `qiskit-machine-learning`, `scikit-learn` and `pandas`) in their first code
  cell. Keep the `.csv` datasets in the same folder as the notebooks.

## Getting the material

With git:

```bash
git clone https://github.com/ilsinay/Quantum-Computing-Spring-School-2026.git
cd Quantum-Computing-Spring-School-2026
```

To fetch any updates, run `git pull` inside that folder.

Without git, use **Code → Download ZIP** on the
[repository page](https://github.com/ilsinay/Quantum-Computing-Spring-School-2026)
and unzip it. Download it again to get any updates.

## Repository layout

```
setup/                                        Setup guide and environment check notebook
session-01-basic-quantum-algorithms/          Lecture 1 slides
session-02-python-for-quantum-computing/      Python for Quantum Computing: notebook and PDF notes
session-04-qiskit-lab-1/                      Qiskit Lab I: notebook and PDF notes
session-05-qiskit-lab-2/                      Qiskit Lab II: notebook and PDF notes
session-06-07-variational-quantum-algorithms/ VQA I and II: slides and handwritten notes
session-08-qiskit-lab-3-vqe/                  Qiskit Lab III: student and solution notebooks
session-09-qiskit-lab-4-qaoa/                 Qiskit Lab IV: notebook and reference paper
session-10-nisq-qml/                          NISQ QML lecture slides
session-11-quantum-simulation/                Quantum simulation lecture slides
session-12-qml-laboratory/                    QML laboratory: notebooks and datasets
session-13-qsim-laboratory/                   QSim laboratory: notebook and PDF notes
```

## Licence

[MIT](LICENSE)
