# CE 222 Final Project: Shear-Deformable Plate Solver

This repository contains the Python implementation for my CE 222 final project.

## Contents

- `CE_222_final_project.ipynb`: full Jupyter notebook implementation
- `CE_222_Final_Report.pdf`: final project report

## Solver Summary

The solver implements a Reissner--Mindlin shear-deformable plate formulation using a heterosis-type Q8/Q9 element:
- Q8 interpolation for transverse displacement `w`
- Q9 interpolation for rotations `theta1`, `theta2`
- Gaussian quadrature for bending and shear stiffness
- Structured mesh generation with rectangular cutout handling
- Line loads, pressure loads, boundary conditions, and post-processing

## Verification Examples

The notebook includes:
- unit tests
- patch tests
- simply supported rectangular plate under uniform pressure
- cantilever plate strip under end line load
- clamped circular plate benchmark
- project mesh convergence study

## Final Project Result

The final computed transverse displacement at point A was:

```text
w_A = -0.34888 mm
