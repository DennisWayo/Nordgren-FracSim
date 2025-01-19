## Introduction
This repository contains the source code, data, and documentation for the research paper titled:
**“Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs”.**

The project combines Physics-Informed Neural Networks (PINNs), Variational Quantum Eigensolver (VQE), and Implicit Numerical Schemes to analyze and optimize hydraulic fracturing processes in shale reservoirs.

### Features
* Physics-Informed Neural Networks (PINNs) for solving Nordgren’s fracture PDE.
* Variational Quantum Eigensolver (VQE) implementation using Qiskit to simulate quantum optimization.
* Implicit Numerical Scheme validation for fracture width evolution.
* Detailed visualization of results (e.g., spatiotemporal evolution, loss curves).
* Comparison of PINNs, VQE, and implicit schemes for accuracy, computational efficiency, and scalability.

## Getting Started

## Prerequisites

Ensure you have the following installed:
* Python 3.9+
* TensorFlow 2.10+
* Qiskit 0.43+
* NumPy, Matplotlib, SciPy

### Installation
1. Clone the repository:
 ```bash
git clone https://github.com/username/Nordgren-FracSim.git
cd Nordgren-FracSim
```

2. Install dependencies:
 ```bash
pip install -r requirements.txt
```
python pinn_training.py

## Usage

1. Physics-Informed Neural Networks (PINNs)

Navigate to the code/pinn directory and run the training script:

 ```bash
python pinn_training.py
```
Generated results:
* Loss curves for training optimizers (Adam, L-BFGS, Newton-CG).
* Spatiotemporal evolution of fracture width.

2. Variational Quantum Eigensolver (VQE)

Navigate to the code/vqe directory and execute the VQE optimization script:

 ```bash
python vqe_optimization.py
```
Generated results:
* Quantum circuit visualization.
* Energy minimization for fracture optimization.

3. Implicit Scheme Validation

Navigate to the code/implicit_scheme directory and run the validation script:

```bash
python implicit_scheme_validation.py
```

## Results

### Comparison of Methods

| Method             | Parameter Values                        | Loss         | Time (s)   | Memory (MB) |
|--------------------|-----------------------------------------|--------------|------------|-------------|
| **PINN (Adam)**    | `E' = 30.0, μ = 5.0, H = 1.0, t = 1.0` | 3.17e-09     | 758.95     | 471.75      |
| **PINN (Adam+L-BFGS)** | `E' = 30.0, μ = 5.0, H = 1.0, t = 2.0` | 7.06e-08     | 734.31     | 328.05      |
| **VQE (SPSA)**     | `E' = 30.0, μ = 8.0, H = 2.0, t = 2.0` | -0.5825+0j   | 1.31       | 0.0         |
| **VQE (L-BFGS)**   | `E' = 30.0, μ = 8.0, H = 2.0, t = 2.0` | -0.5831+0j   | 0.20       | 0.0         |

## Figures

Generated plots and visualizations:
* Fracture width evolution (PINN, VQE, implicit scheme).
* Loss curves for training optimizers.
*	Spatiotemporal contour maps.

## Funders
Nazarbayev University CRP - 
MOHE/UMPSA - 

## Contact

For questions or collaborations:
	•	Author Name: iwayoden@gmail.com
	•	GitHub: [[GitHub Profile Link](https://github.com/DennisWayo)]
