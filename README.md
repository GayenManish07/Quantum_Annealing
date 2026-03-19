# Quantum Annealing for Traveling Salesman Problem (TSP)

## Overview
This project explores solving the **Traveling Salesman Problem (TSP)** using **Quantum Annealing**.

The problem is formulated as a **QUBO (Quadratic Unconstrained Binary Optimization)** and solved using **simulated quantum annealing** via the `OpenJij` library.

The goal is to compare how quantum-inspired methods perform against classical approaches.

---

## Methods Compared
- **Brute Force**  
  Finds the exact optimal solution but is computationally expensive.

- **Quantum Annealing (OpenJij)**  
  Uses a probabilistic approach to find near-optimal solutions efficiently.

- **Greedy (Nearest Neighbor)**  
  Fast heuristic with lower accuracy.

---

## Implementation Summary
- Encoded TSP as a **QUBO matrix** using binary variables  
- Added **penalty constraints** to enforce valid tours  
- Used `OpenJij`'s `SASampler` to simulate annealing  
- Benchmarked performance across different city sizes  
- Visualized **distance vs runtime** using `matplotlib`

---

## Key Result
For 11 cities:
- **Brute Force:** Optimal solution (~169s)  
- **Quantum Annealing:** Near-optimal (~7.5s)  
 Shows a strong **speed vs optimality trade-off**

