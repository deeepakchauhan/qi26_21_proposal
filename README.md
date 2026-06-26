# 🔬 Quantum Harmonic Oscillator Ground State Estimator

**Author:** Deepak Chauhan
**Program:** Integrated MSc Physics, NIT Surat
**Project:** QIntern'26 Proposal — Phase 2

---

## What This Project Does

This project implements a **Variational Quantum Eigensolver (VQE)**
to estimate the ground state energy of the Quantum Harmonic Oscillator (QHO):

$$E_0 = \frac{1}{2}\hbar\omega$$

using IBM's `qiskit-nature` library, executed on `AerSimulator`.

---

## Tech Stack

| Tool | Version | Role |
|------|---------|------|
| Qiskit | 2.4.1 | Core quantum SDK |
| qiskit-nature | 0.7.2 | Bosonic Hamiltonian construction |
| qiskit-aer | 0.15.0 | Cloud simulator backend |
| ipywidgets + Voilà | latest | Interactive visual dashboard |
| COBYLA (scipy) | latest | Classical optimizer |

---

## Results

| Method | E₀ (ℏω units) | Error |
|--------|--------------|-------|
| Exact (NumPy) | 0.50000000 | — |
| VQE (COBYLA) | 0.50000000 | < 10⁻⁸ |

VQE recovered the ground state energy to **machine precision**
in ~23 optimizer iterations.

---

## Project Structure
qi26_21_proposal/

├── QHO_Notebook.ipynb         

├── requirements.txt       

└── README.md              
