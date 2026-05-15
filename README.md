# Nystrom

![MATLAB](https://img.shields.io/badge/-MATLAB-0076A8?logo=mathworks&logoColor=white)

# 2D Electromagnetic scattering (TM)

## Nyström (Electric Field Integral Equation - Perfect Electric Conductors) + Richmond (Volume Integral Equation - Dielectric)

This repository contains MATLAB implementations of two classical integral‑equation solvers for 2D electromagnetic scattering under TM polarization:

- Nyström Electric Field Integral Equation (EFIE) for perfectly conducting cylinders, using Colton–Kress trigonometric quadrature for the periodic logarithmic kernel - Martensen–Kussmaul splitting of the single-layer operator

- Richmond Volume Integral Equation (VIE) for dielectric cylinders of arbitrary cross section

Both solvers include analytical reference solutions (cylindrical harmonics) for validation.
