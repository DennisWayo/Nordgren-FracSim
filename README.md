# Introduction
This repository contains the source code, data, and documentation for the research paper titled:
**“Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs”.**

The project combines Physics-Informed Neural Networks (PINNs), Variational Quantum Eigensolver (VQE), and Implicit Numerical Schemes to analyze and optimize hydraulic fracturing processes in shale reservoirs.

## Features
* Physics-Informed Neural Networks (PINNs) for solving Nordgren’s fracture PDE.
* Variational Quantum Eigensolver (VQE) implementation using Qiskit to simulate quantum optimization.
* Implicit Numerical Scheme validation for fracture width evolution.
* Detailed visualization of results (e.g., spatiotemporal evolution, loss curves).
* Comparison of PINNs, VQE, and implicit schemes for accuracy, computational efficiency, and scalability.

 # Reporsitory Structure
 root/
├── README.md                # Repository overview
├── LICENSE                  # License for the repository
├── data/                    # Training and validation datasets
├── code/                    # Source code
│   ├── pinn/                # PINN implementation
│   ├── vqe/                 # VQE implementation
│   ├── implicit_scheme/     # Implicit scheme validation
├── figures/                 # Generated figures for analysis
├── results/                 # Stored results for PINN and VQE
├── docs/                    # Additional documentation and research paper
└── requirements.txt         # Python dependencies

# Getting Started

## Prerequisites

Ensure you have the following installed:
* Python 3.9+
* TensorFlow 2.10+
* Qiskit 0.43+
* NumPy, Matplotlib, SciPy

## Installation
	1.	Clone the repository:
 ```bash
git clone https://github.com/username/Nordgren-Fracture-Simulation.git
cd Nordgren-Fracture-Simulation
```

	2.	Install dependencies:
 ```bash
pip install -r requirements.txt
```

# Usage

1. Physics-Informed Neural Networks (PINNs)

Navigate to the code/pinn directory and run the training script:
