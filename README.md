[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Build Status](https://img.shields.io/badge/PINN-yes-green)
![Build Status](https://img.shields.io/badge/VQE-yes-green)
![Contributions](https://img.shields.io/badge/contributions-welcome-gold)
![GitHub issues](https://img.shields.io/github/issues/DennisWayo/Nordgren-FracSim)
![GitHub forks](https://img.shields.io/github/forks/DennisWayo/Nordgren-FracSim)
![GitHub stars](https://img.shields.io/github/stars/DennisWayo/Nordgren-FracSim)


## Introduction
This repository contains the python scripts, data, and documentation for the research paper titled:
**“Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs”.**

The project combines Physics-Informed Neural Networks (PINNs), Variational Quantum Eigensolver (VQE), and Implicit Numerical Schemes to analyze and optimize hydraulic fracturing processes in shale reservoirs.

### Features
* Physics-Informed Neural Networks (PINNs) for solving Nordgren’s fracture PDE.
* Variational Quantum Eigensolver (VQE) implementation using Qiskit to simulate quantum optimization.
* Implicit Numerical Scheme validation for fracture width evolution.
* Detailed visualization of results (e.g., spatiotemporal evolution, loss curves).
* Comparison of PINNs, VQE, and implicit schemes for accuracy, computational efficiency, and scalability.

## Getting Started

### Prerequisites

* Google Colab & Qbraid
* Here is a video of how to get started..


### Usage

**1. Physics-Informed Neural Networks (PINNs)- Google Colab**

Navigate to the code/pinn directory and run the training script:

 ```python
 nordgren_pinn.ipynb
```
Generated results:
* Loss curves for training optimizers (Adam, L-BFGS, Newton-CG).
* Spatiotemporal evolution of fracture width.

**2. Variational Quantum Eigensolver (VQE)- Qbraid**

Navigate to the code/vqe directory and execute the VQE optimization script:

 ```python
 nordgren_vqe.ipynb
```
Generated results:
* Quantum circuit visualization.
* Energy minimization for fracture optimization.

**3. Implicit Scheme Validation**

Navigate to the code/implicit_scheme directory and run the validation script:

```python
 Implicitvalid.ipynb
```

## Results

### Comparison of Methods

| Method             | Parameter Values                        | Loss         | Time (s)   | Memory (MB) |
|--------------------|-----------------------------------------|--------------|------------|-------------|
| **PINN (Adam)**    | `E' = 30.0, μ = 5.0, H = 1.0, t = 1.0` | 3.17e-09     | 758.95     | 471.75      |
| **PINN (Adam+L-BFGS)** | `E' = 30.0, μ = 5.0, H = 1.0, t = 2.0` | 7.06e-08     | 734.31     | 328.05      |
| **VQE (SPSA)**     | `E' = 30.0, μ = 8.0, H = 2.0, t = 2.0` | -0.5825+0j   | 1.31       | 0.0         |
| **VQE (L-BFGS)**   | `E' = 30.0, μ = 8.0, H = 2.0, t = 2.0` | -0.5831+0j   | 0.20       | 0.0         |

### Figures

Generated plots and visualizations:
* Fracture width evolution (PINN, VQE, implicit scheme).
* Loss curves for training optimizers.
* Spatiotemporal contour maps.

### Funders
This research was funded by Nazarbayev University's Collaborative Research Project (CRP) grant number 111024CRP2014 [Associate Professor Sonny Irawan & Professor Randy Hazlett] and supported by Universiti Malaysia Pahang Al-Sultan Abdullah (UMPSA) through the MOHE FRGS grant scheme (FRGS/1/2023/TK08/UMP/02/13) and the Faculty of Chemical \& Process Engineering Technology (RDU230146) [Dr Zulkifli Noor]

### Contributors
Special thanks to Dr. Mudasar Zafar, Mrs Shynar Juziyeva, Professor Camila Martins Saporetti and Professor Leonardo Goliatt

### Cite preprint version as;
* Wayo, D. D. K., Irawan, S., Noor, M. Z. B. M., Zafar, M., Juziyeva, S., Saporetti, C. M., ... & Hazlett, R. (2025). Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs.

```python
@article{wayo2025nordgren,
  title={Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs},
  author={Wayo, Dennis Delali Kwesi and Irawan, Sonny and Noor, Mohd Zulkifli Bin Mohamad and Zafar, Mudasar and Juziyeva, Shynar and Saporetti, Camila Martins and Goliatt, Leonardo and Hazlett, Randy},
  year={2025},
doi={https://doi.org/10.21203/rs.3.rs-5947578/v1}
}
```

### Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

### Contact
For questions, reach out via email(iwayoden@gmail.com) or GitHub discussions.
