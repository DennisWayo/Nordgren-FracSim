[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Build Status](https://img.shields.io/badge/PINN-yes-green)
![Build Status](https://img.shields.io/badge/VQE-yes-green)
![Contributions](https://img.shields.io/badge/contributions-welcome-gold)
![GitHub issues](https://img.shields.io/github/issues/DennisWayo/Nordgren-FracSim)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15043799.svg)](https://doi.org/10.5281/zenodo.15043799)
![GitHub forks](https://img.shields.io/github/forks/DennisWayo/Nordgren-FracSim)
![GitHub stars](https://img.shields.io/github/stars/DennisWayo/Nordgren-FracSim)



This repository contains the python scripts, data, and documentation for the research paper titled:
**“Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs”.**

The project combines Physics-Informed Neural Networks (PINNs), Variational Quantum Eigensolver (VQE), and Implicit Numerical Schemes to analyze and optimize hydraulic fracturing processes in shale reservoirs.

### Features
* Physics-Informed Neural Networks (PINNs) for solving Nordgren’s fracture PDE.
* Variational Quantum Eigensolver (VQE) implementation using Qiskit to simulate quantum optimization.
* Implicit Numerical Scheme validation for fracture width evolution.
* Detailed visualization of results (e.g., spatiotemporal evolution, loss curves).
* Comparison of PINNs, VQE, and implicit schemes for accuracy, computational efficiency, and scalability.

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

**Cite preprint version as;**

* Wayo, D. D. K., Irawan, S., Noor, M. Z. B. M., Zafar, M., Juziyeva, S., Saporetti, C. M., ... & Hazlett, R. (2025). Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs.

```bibtex
@article{wayo2025nordgren,
  title={Nordgren Physics-Informed Neural Networks to Variational Quantum Eigensolver: Advancing Hydraulic Fracturing Simulations in Shale Reservoirs},
  author={Wayo, Dennis Delali Kwesi and Irawan, Sonny and Noor, Mohd Zulkifli Bin Mohamad and Zafar, Mudasar and Juziyeva, Shynar and Saporetti, Camila Martins and Goliatt, Leonardo and Hazlett, Randy},
  year={2025},
doi={https://doi.org/10.21203/rs.3.rs-5947578/v1}
}
```

**Cite code version as;**

Nordgren-FracSim Python code is the framework used for this paper, researchers are free to modify and cite for various fracturing studies.

```bibtex
@software{wayo_2025_15043799,
  author       = {Wayo, Dennis Delali Kwesi},
  title        = {Nordgren-FracSim: Python-Based Fracture Simulation
                   Using the Nordgren Model
                  },
  month        = mar,
  year         = 2025,
  publisher    = {Zenodo},
  version      = {1.0},
  doi          = {10.5281/zenodo.15043799},
  url          = {https://doi.org/10.5281/zenodo.15043799},
}
```

### Funders
- Nazarbayev University's Collaborative Research Project (111024CRP2014)
- Universiti Malaysia Pahang Al-Sultan Abdullah (UMPSA) through the MOHE FRGS grant scheme (FRGS/1/2023/TK08/UMP/02/13)
- Faculty of Chemical & Process Engineering Technology (RDU230146)

### Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

### Contact
For questions, reach out via email(iwayoden@gmail.com) or GitHub discussions.
