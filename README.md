# Poisson Equation with Weak Dirichlet Boundary Conditions using FEniCSx

This project demonstrates how to solve the Poisson equation using the finite element method with **weak imposition of Dirichlet boundary conditions** via **Nitsche's method**. The implementation is based on the [FEniCSx](https://fenicsproject.org/) (Dolfinx) library, with visualization powered by [PyVista](https://docs.pyvista.org/).

---

## 📘 Problem Description

We solve the Poisson equation:

$$
-\Delta u = f \quad \text{in } \Omega = [0,1]^2
$$

with a manufactured solution:

$$
u(x, y) = 1 + x^2 + 2y^2
$$

Dirichlet boundary conditions are imposed **weakly** using **Nitsche's method**.

---

## 🛠️ Features

- Solves a 2D Poisson problem on a unit square mesh
- Uses **Nitsche’s method** to weakly impose Dirichlet boundary conditions
- Computes **L²-norm** and **maximum-norm** of the numerical error
- Visualizes the finite element solution using **PyVista**
- Fully documented and commented notebook

---

## 📦 Requirements

- FEniCSx / Dolfinx
- `mpi4py`
- `numpy`
- `pyvista`

Install Python dependencies:

```bash
pip install numpy mpi4py pyvista
