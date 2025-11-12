# Algorithmic-Strategies-in-Real-World-Problems

Course: Design and Analysis of Algorithms (ENCA351) - Semester V
LAB ASSIGNMENT - 2
## Overview
This notebook demonstrates 4 algorithmic strategies applied to real-world problems:
1. TV Commercial Scheduling — Greedy (Job sequencing)
2. 0/1 Knapsack — Dynamic Programming
3. Sudoku Solver — Backtracking
4. Password Cracking (naive) — Brute Force

### Summary Table & Analysis

| **Problem** | **Algorithmic Strategy** | **Time Complexity** | **Space Complexity** | **Memory Usage (approx.)** | **Execution Time (sample)** | **Scalability** | **Remarks** |
|--------------|---------------------------|---------------------|----------------------|-----------------------------|------------------------------|------------------|--------------|
| **TV Commercial Scheduling** | Greedy (Job Sequencing with Deadlines) | O(n log n + n·D) where D = max deadline | O(D) | ~5–10 MB | 0.002 s for 50 ads |  Excellent — scales almost linearly | Efficient for large inputs due to simple sorting and linear pass |
| **0/1 Knapsack** | Dynamic Programming (Bottom-Up) | O(n × W) where W = capacity | O(n × W) | ~15–25 MB | 0.03 s for n = 30, W = 100 |  Moderate — depends on capacity size | Performs well for small W but grows fast with larger capacities |
| **Sudoku Solver** | Backtracking (DFS Search) | O(9ⁿ) worst-case | O(1) (ignoring recursion stack) | ~10–20 MB | 0.05 s for easy puzzle, > 1 s for hard puzzle |  Limited — exponential growth | Works for standard 9×9, slow for larger puzzles |
| **Password Cracker** | Brute Force (Exhaustive Search) | O(k^L) where k = charset size, L = length | O(1) | ~2–5 MB | 0.001 s (L=2), > 10 s (L=5) |  Poor — exponential blow-up | Demonstrates inefficiency of brute-force methods |


## How to run
1. Clone the repo.
2. Create & activate Python virtual environment:
   python3 -m venv venv
   source venv/bin/activate
3. Install requirements:
   pip install -r requirements.txt
4. Launch Jupyter:
   jupyter notebook
5. Open `algo_strategies_notebook.ipynb` and run cells.

## Files
- `algo_strategies_notebook.ipynb`: main notebook with code, plots, and explanation

## Notes & Academic Integrity
This is an individual assignment. All code and writeups are authored by <Kartik Singh>.
References: CLRS (Introduction to Algorithms), Python docs, matplotlib docs.

