# Running the notebooks in Google Colab

[Google Colab](https://colab.research.google.com/) runs Jupyter notebooks in
your browser on Google's machines, so you don't need to install Python,
Anaconda or anything else. You only need a Google account.

Colab is a good fallback if you can't install the
[setup guide](pre_school_setup_guide.pdf) environment on your own laptop, or
if you want to try a notebook quickly. Your own installation is still better
for longer work: Colab sessions time out when idle, and everything you install
or download disappears when the session ends.

## 1. Open a notebook

Click a notebook's link below. It opens a read-only copy in Colab.

| Session | Notebook | Link | Packages |
|---|---|---|---|
| Setup | Environment check | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/setup/00_environment_check.ipynb) | Install cell below |
| 1 | Python for Quantum Computing | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-01-python-for-quantum-computing/01_intro_python_for_quantum_computing.ipynb) | Install cell below |
| 4 | Qiskit Lab I | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-04-qiskit-lab-1/04_intro_quantum_computing_qiskit.ipynb) | Install cell below |
| 5 | Qiskit Lab II | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-05-qiskit-lab-2/05_quantum_algorithms_qiskit.ipynb) | Install cell below |
| 8 | Qiskit Lab III: VQE (student) | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-08-qiskit-lab-3-vqe/vqe_tutorial_student.ipynb) | Has its own install cell |
| 8 | Qiskit Lab III: VQE (solutions) | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-08-qiskit-lab-3-vqe/vqe_tutorial_solution.ipynb) | Has its own install cell |
| 9 | Qiskit Lab IV: QAOA | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-09-qiskit-lab-4-qaoa/05_QAOA_MaxCut.ipynb) | Install cell below |
| 12 | QML laboratory: QSVM (iris) | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-12-qml-laboratory/qsvm_iris_qiskit-2.ipynb) | Has its own install cell |
| 12 | QML laboratory: QNN (penguins) | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-12-qml-laboratory/qnn_penguins_qiskit.ipynb) | Has its own install cell |
| 12 | QML laboratory: QCNN (pulsars) | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-12-qml-laboratory/qcnn_pulsars_qiskit.ipynb) | Has its own install cell; also download the dataset (below) |
| 13 | QSim laboratory | [Open in Colab](https://colab.research.google.com/github/ilsinay/Quantum-Computing-Spring-School-2026/blob/main/session-13-qsim-laboratory/13_quantum_simulation_qiskit.ipynb) | Install cell below |

To open any other notebook from this repository: in Colab choose
**File → Open notebook → GitHub**, paste
`https://github.com/ilsinay/Quantum-Computing-Spring-School-2026`, and pick
the notebook from the list.

## 2. Install Qiskit

Colab already includes NumPy, SciPy, Matplotlib, pandas, scikit-learn and
networkx, but not Qiskit. For notebooks marked "Install cell below", add a
code cell at the very top (**Insert → Code cell**), paste this in, and run it
before anything else:

```python
%pip install --quiet qiskit qiskit-aer pylatexenc
```

The VQE and QML notebooks already start with their own install cell, so just
run that first.

If Colab shows a **Restart session** button after installing, click it, then
carry on from the next cell. You don't need to run the install cell again
until your next session.

You need to install again every time you start a new Colab session.

## 3. Data files (QML laboratory)

- **QCNN (pulsars)** reads `HTRU_2.csv` from the notebook's folder, which
  Colab doesn't provide. Before the cell that loads the data, run:

  ```python
  !wget -q https://raw.githubusercontent.com/ilsinay/Quantum-Computing-Spring-School-2026/main/session-12-qml-laboratory/HTRU_2.csv
  ```

- **QNN (penguins)** downloads its dataset automatically if the file is
  missing, so it needs nothing extra.

## 4. Save your work

The copy Colab opens is not saved anywhere. To keep your changes, choose
**File → Save a copy in Drive** before you start editing. Your copy then lives
in the `Colab Notebooks` folder of your Google Drive.

## Things that behave differently in Colab

- **Links between tutorials** (for example "In Session 4 …") point to files in
  this repository, so they don't open in Colab. Use the table above instead.
- **The QAOA notebook's MaxCut figure** doesn't show, because the image file
  isn't copied into Colab. The code is unaffected.
- **The PDF notes and lecture slides** open directly on GitHub; you don't need
  Colab for those. See the [README](../README.md).
