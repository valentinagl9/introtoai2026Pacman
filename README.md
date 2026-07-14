# Pacman AI Search Project

## Overview

This project was developed as part of the Introduction to Artificial Intelligence course at Ascencia University.

The project is based on the UC Berkeley Pacman AI framework and focuses on implementing classical Artificial Intelligence search algorithms to solve maze navigation problems.

The implemented search strategies are:

- Depth-First Search (DFS)
- Breadth-First Search (BFS)
- Uniform Cost Search (UCS)
- A* Search

Each algorithm uses a different search strategy to explore the maze and find a path for the Pacman agent.

---

## Implemented Algorithms

### Depth-First Search (DFS)

Depth-First Search explores the deepest nodes first before backtracking. It uses a stack data structure to manage the exploration process.

### Breadth-First Search (BFS)

Breadth-First Search explores nodes level by level using a queue. It guarantees finding the shortest path when all actions have the same cost.

### Uniform Cost Search (UCS)

Uniform Cost Search expands the node with the lowest total path cost. It uses a priority queue to find the optimal path based on movement cost.

### A* Search

A* Search combines the cost already traveled with a heuristic estimation to efficiently find an optimal solution.

---

## Project Structure

```
introtoai2026Pacman/

├── search.py
├── searchAgents.py
├── pacman.py
├── util.py
├── layouts/
└── README.md
```

### Main Files

- `search.py`  
  Contains the implementation of the AI search algorithms.

- `searchAgents.py`  
  Contains the Pacman agents that use the implemented search strategies.

- `pacman.py`  
  Main program used to launch the Pacman environment.

- `layouts/`  
  Contains maze configurations used to test the algorithms.

---

## Running the Project

The different search algorithms can be executed using the following commands.

### Breadth-First Search (BFS)

```bash
python3 pacman.py -l tinyMaze -p SearchAgent -a fn=bfs
```

### Depth-First Search (DFS)

```bash
python3 pacman.py -l tinyMaze -p SearchAgent -a fn=dfs
```

### Uniform Cost Search (UCS)

```bash
python3 pacman.py -l tinyMaze -p SearchAgent -a fn=ucs
```

### A* Search

```bash
python3 pacman.py -l tinyMaze -p SearchAgent -a fn=astar
```

---

## Testing

The algorithms are tested using different Pacman maze environments, including:

- `tinyMaze`
- `mediumMaze`

Each search strategy explores the environment differently depending on its implementation and search approach.

---

## Technologies

- Python 3
- UC Berkeley Pacman AI Framework

---

## Author

Your Name  
Introduction to Artificial Intelligence 2026  
Ascencia University