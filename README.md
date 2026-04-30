# Nystrom

![MATLAB](https://img.shields.io/badge/-MATLAB-0076A8?logo=mathworks&logoColor=white)

# EFIE Nyström Solver for 2D PEC Cylinder (TM\_z)

This repository contains a MATLAB implementation of a Nyström discretization of the Electric Field Integral Equation (EFIE) for 2D scattering by a perfectly conducting circular (or elliptical) cylinder under TM\_z polarization.

The method combines:

- Colton–Kress trigonometric quadrature for the periodic logarithmic kernel
- Martensen–Kussmaul splitting of the single-layer operator
- A Nyström scheme where the same nodes and weights are used for:
  - EFIE discretization
  - Far-field evaluation

## Files

- `src/main_efie_nystrom_circle.m`  
  Main script: builds the EFIE operator, solves for the surface current, and compares:
  - Numerical current vs. analytic series (cylindrical harmonics)
  - Numerical far-field vs. analytic Mie-series far-field

- `src/RColtonKress.m`  
  Colton–Kress trigonometric weights for the periodic logarithmic kernel.

- `src/current_circle.m`  
  Analytic TM\_z surface current on a circular PEC cylinder (Mie-series).

- `src/farfield_circle.m`  
  Analytic TM\_z far-field pattern for a circular PEC cylinder (Mie-series).

## Usage

1. Open MATLAB in the repository root.
2. Add the `src` folder to the path:
   ```matlab
   addpath('src');
3. Run: main_efie_nystrom_circle

