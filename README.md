# nk-3eq-model-replication

This repository replicates the core results of the paper:

**"The Analytics of the New Keynesian 3-Equation Model"**  
Jean-Christophe Poutineau, Karolina Sobczak, Gauthier Vermandel  
_Economics and Business Review_, Vol. 1 (15), No. 2, 2015, pp. 110–129  
Originally published by the University of Poznan.

---

## 📌 Purpose

This project provides a Julia-based replication of the canonical New Keynesian 3-equation model using:

- [`MacroModelling.jl`](https://github.com/IMFS-MMB/MacroModelling.jl) – for solving DSGE models
- [`StatsPlots.jl`](https://github.com/JuliaPlots/StatsPlots.jl) – for visualizing impulse response functions and results

The original Dynare/MATLAB code is translated into idiomatic Julia code using modern macroeconomic modeling tools.  
It is particularly suited for students, researchers, and instructors seeking transparent and reproducible macroeconomic model implementations.

---

## 📘 Model Description

We implement a simple dynamic New Keynesian model composed of:

1. **IS Curve (Aggregate Demand Equation)**
2. **New Keynesian Phillips Curve (Aggregate Supply Equation)**
3. **Taylor Rule (Monetary Policy Rule)**

These equations represent the core of modern macroeconomic DSGE frameworks and provide a flexible structure for shock analysis and policy evaluation.

---

## 🧪 What This Repository Does

- Defines the structural equations of the model using `MacroModelling.jl`
- Calibrates model parameters consistent with the paper
- Introduces three shocks:
  - **Demand shock**
  - **Supply (cost-push) shock**
  - **Monetary policy shock**
- Computes **impulse response functions (IRFs)**
- Visualizes the effects on:
  - Output gap  
  - Inflation  
  - Nominal interest rate  

---

## 🛠 How to Run

### 📦 Dependencies

Install required Julia packages:

```julia
using Pkg
Pkg.add(["MacroModelling", "StatsPlots"])
```
