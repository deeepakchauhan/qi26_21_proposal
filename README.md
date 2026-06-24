# Quantum Harmonic Oscillator Ground-State Estimation using VQE

## Overview

This project implements the Variational Quantum Eigensolver (VQE) to estimate the ground-state energy of a Quantum Harmonic Oscillator (QHO) using Qiskit Nature.

The workflow demonstrates the complete hybrid quantum-classical pipeline:

BosonicOp → BosonicLinearMapper → SparsePauliOp → Variational Ansatz → Estimator → COBYLA Optimizer

The VQE result is compared against the exact analytical solution and exact diagonalization results.

---

## Objectives

* Construct the QHO Hamiltonian in second quantization.
* Map bosonic operators to qubit operators.
* Implement a variational quantum circuit (ansatz).
* Optimize circuit parameters using COBYLA.
* Estimate the ground-state energy using VQE.
* Compare VQE results with exact solutions.

---

## Technologies Used

* Python
* Qiskit
* Qiskit Nature
* NumPy
* SciPy
* Matplotlib

---

## Future Work

* Multi-mode harmonic oscillators
* Coupled oscillators
* Vibrational quantum chemistry
* Execution on IBM Quantum hardware
* Advanced ansatz design and error mitigation

---

## Author

Deepak Chauhan

Integrated MSc Physics 
SVNIT Surat
