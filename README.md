# Traveling Ethiopia Problem

## Contributors

* Abel Tadesse
* GSR/2025/17

## Overview

The **Traveling Ethiopia Problem** is an interactive application built with Streamlit to solve various graph traversal challenges on Ethiopia's road network. It leverages algorithms like BFS, DFS, Weighted BFS, Dijkstra, A*, and more. The application features:

* **Pathfinding** : Determine optimal paths between cities.
* **All-Pairs Shortest Paths** : Visualize shortest paths between all cities.
* **Traverse All Cities** : Visit every city exactly once or allow repeated visits.

---

## Features

### 1. Traveling Ethiopia Problem

* **Description** : This module solves pathfinding problems between two selected cities using different search algorithms.
* **Inputs** :
* Start City
* Goal City (optional)
* Strategy (BFS, DFS, Weighted BFS, Dijkstra, A*)
* **Outputs** :
* Path and its cost
* Visualization of the road network with the path highlighted.

### 2. All Pairs Shortest Paths

* **Description** : Computes and visualizes shortest paths between all pairs of cities.
* **Algorithms** :
* **Floyd-Warshall** : Computes the shortest path matrix for all city pairs.
* **Bellman-Ford** : Computes shortest paths from a selected city to all other cities.
* **Outputs** :
* A matrix representation of shortest paths.
* Visualization for Bellman-Ford as a row matrix for the selected city.

### 3. Traverse All Cities

* **Description** : Traverses all cities in Ethiopia starting from a selected city.
* **Modes** :
* **Only Once Visit** : Ensures each city is visited exactly once.
* **Repeated Visit** : Allows revisiting cities if necessary.
* **Inputs** :
* Start City
* Strategy (BFS, DFS)
* **Outputs** :
* Path taken to traverse all cities.
* Visualization of the traversal path.

---

## How to Use

### 1. Launching the Application

Run the application using Streamlit:

```bash
streamlit run main.py
```

### 2. Navigation

* Use the **Dashboard** on the sidebar to select a feature:
  1. **Traveling Ethiopia Problem**
  2. **All Pairs Shortest Paths**
  3. **Traverse All Cities**

### 3. Inputs and Outputs

#### Traveling Ethiopia Problem

* Select start and goal cities.
* Choose a strategy.
* View the computed path and its cost.
* Visualize the path on the road network.

#### All Pairs Shortest Paths

* Run Floyd-Warshall for all pairs.
* Select a start city and run Bellman-Ford for shortest paths from that city.
* Visualize the results as a matrix.

#### Traverse All Cities

* Select a start city and strategy.
* Choose between "Only Once Visit" or "Repeated Visit" traversal modes.
* View the traversal path and its visualization.

---

## Algorithms Used

### Pathfinding Algorithms

1. **BFS** (Breadth-First Search): Finds the shortest path in terms of the number of edges.
2. **DFS** (Depth-First Search): Explores paths deeply to find feasible paths.
3. **Weighted BFS** : Uses cumulative path cost as a priority heuristic.
4. **Dijkstra** : Finds the shortest path based on edge weights.
5. **A** *: Optimized pathfinding with a heuristic function.

### All-Pairs Shortest Path Algorithms

1. **Floyd-Warshall** : Computes shortest paths between all pairs of nodes.
2. **Bellman-Ford** : Computes shortest paths from a single source node, handling negative edge weights.

### Traversal Algorithms

1. **Traverse All Cities** : Visits every city exactly once.
2. **Traverse All Cities with Revisits** : Visits every city, allowing revisits if necessary.

---

## Visualization

* **Graph Visualizations** : Highlights paths on Ethiopia's road network.
* **Matrix Visualizations** :
* Full matrix for Floyd-Warshall.
* Row matrix for Bellman-Ford from a specific start city.

---

## Requirements

* Python 3.7+
* Streamlit
* NumPy
* Matplotlib
* Networkx

Install dependencies:

```bash
pip install streamlit numpy matplotlib
```

```bash
pip install -r requirements.txt
```
