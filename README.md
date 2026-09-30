# Comparison of Single-Solution-Driven and Population-Driven Algorithm Performance in Providing Solutions to TSP
Coursework Submission (edited and merged) for MSc Artificial Intelligence @ UWE

### Problem Definition
The Travelling Salesman Problem (TSP): a salesman must visit a series of cities exactly once and return home.
- Route: Sequence of cities visited from start to finish
- Solution: A proposed route

## Main Comparison
Simulated Annealing (SA) vs Genetic Algorithm (GA):
- Shortest Average Route
- Robustness
- Execution Time

## Contents:
- Preliminary experiments using a few (mainly) single-solution algorithms for 'solving' TSP - best-performing chosen
  -  Hill Climbing (Steepest Ascent)
  -  Simulated Annealing
  -  TABU
  -  Genetic Algorithm
- SA vs GA
  - 10-seed runs each
  - Repeated over 5 problem spaces of varying size
  - Analysis & Discussion

### Inheritance & Operators 
- The algorithms inherit basic functions from the main TSP problem class:
  - TSP environment set-up, including distance matrix between cities,
  - Objective Function
- Also included in the TSP class are shared operators and visualisation functions:
  - Generate an initial random solution
  - City Swaps
  - Convergence graph
  - Solution visualisation graphs  

# Main Findings
- City swapping operators (simple-swap vs 2-opt) appear to have a greater impact on performance than the specific algorithm selected.
- Overall, GA generally produces better solutions (avg. shortest route) than SA, with greater consistency (std.).
- SA is much faster than GA. It can produce 'acceptable' solutions in a fraction of the time, with little variance in performance over problem size.
