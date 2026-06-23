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

## Methodology

1. Construct the bosonic Hamiltonian

   H = ħω(a†a + 1/2)

2. Map the Hamiltonian to qubits using BosonicLinearMapper.

3. Create a parameterized TwoLocal ansatz.

4. Compute expectation values using Qiskit's Estimator primitive.

5. Optimize variational parameters using COBYLA.

6. Compare the optimized energy with the exact ground-state energy.

---

## Results

Ground-State Energy:

E₀ = 0.5 ħω

VQE Energy:

E_VQE = 0.5 ħω

Absolute Error:

|E_VQE − E₀| = 0

The variational algorithm successfully recovered the exact ground-state energy on AerSimulator.

---

## Visualizations

The project includes:

* Energy convergence plot
* VQE vs exact energy comparison
* Ansatz circuit visualization
* Energy landscape analysis
* Bloch sphere representation

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
