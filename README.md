# MARS-PATH-PLANNING-AI
Route planning and optimization on Mars using AI algorithms such as A*, Greedy, CSP, and Simulated Annealing, applied to real terrain maps.

# Mars Path Planning & Charging Station Optimization 

This project explores autonomous route planning and infrastructure optimization on the Martian surface using artificial intelligence techniques. It includes search algorithms for navigation and constraint-based optimization for charging station placement, all applied to real NASA Mars terrain data.

## Project Components

### Route Planning
We implemented and compared various search algorithms to find optimal paths on Martian maps:
- A* (A-star)
- Breadth-First Search (BFS)
- Uniform Cost Search
- Greedy Best-First Search
- Best-First Search

Each was tested on multiple start-end coordinate pairs, analyzing time, distance, and performance trade-offs.

### Charging Station Optimization
We designed a system for positioning drone charging stations that balance:
- **Coverage** (maximize visible tiles)
- **Separation** (≥1 km between stations)
- **Accessibility** (≤3 km to nearest station)

We used:
- **CSP (Constraint Satisfaction Problem)** with backtracking
- **Greedy Search** to iteratively improve coverage
- **Simulated Annealing** for global optimization

---

## Key Takeaways

- A* consistently produced shorter routes but with higher computation time.
- Greedy search was fastest but often suboptimal in path quality.
- CSP ensured rule-based feasibility for station placement.
- Simulated Annealing outperformed Greedy in optimizing station coverage.

---

## 🛠 Technologies & Tools

- **Languages**: Python, NumPy, Matplotlib
- **Libraries**: simpleai, CSP modules, custom heuristics
- **Concepts**: Search algorithms, local search, constraint satisfaction, optimization, pathfinding

---


## Disclaimer

This project was developed as a university AI capstone for educational and demonstrative purposes. Terrain maps are sourced from public NASA repositories.

