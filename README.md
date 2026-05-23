# Constrained Multiphysics PINN for Piezoelectric Tensor Discovery

Code repository for the paper: *Inverse Discovery of Shear Piezoelectric Coupling in Anisotropic Media via Topologically Constrained Multiphysics Neural Networks*.

This repository implements a Physics-Informed Neural Network (PINN) with an exact $t^2$ temporal and spatial distance function topology to bypass initial-state electrostatic singularities (the Poisson explosion) in coupled electro-elastodynamics.

## Requirements
- Python 3.9+
- PyTorch 2.0+
- NumPy, SciPy

## Usage
Run the main training pipeline to execute the 2-stage (Adam -> L-BFGS) inverse discovery of the dimensionless $e_{15}$ shear parameter.

```bash
python src/train.py
