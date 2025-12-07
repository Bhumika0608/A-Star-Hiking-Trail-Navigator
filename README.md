# A-Star-Hiking-Trail-Navigator
This project implements the A* (A-star) search algorithm for intelligent pathfinding across hiking terrains. Unlike traditional path planners that only consider shortest distance, this navigator balances **distance**, **elevation**, **terrain difficulty**, and **scenic preference** to compute the most optimal hiking routes based on user-defined priorities.

---

## Project Overview

A* is a popular pathfinding algorithm that evaluates:

- **g(n):** Cost from start node to current node  
- **h(n):** Estimated cost from current node to the goal  
- Total score: **f(n) = g(n) + h(n)**

In this application, A* is adapted for real-world hiking environments by incorporating:

- Terrain difficulty (trails, flat ground, forests, mountains, water)
- Elevation changes (uphill/downhill penalties)
- Scenic viewpoints and interest points with cost reductions
- User-adjustable weights to tailor the experience

This provides hikers with more realistic and personalized routing options.

---

## Key Algorithm Principles

✔️ **Optimality** ensured with an admissible heuristic (Euclidean distance)  
✔️ **Efficiency** through priority queue–based node selection  
✔️ **Flexibility** with customizable cost functions  
⚠️ Space complexity grows with map size because nodes must be stored in open/closed sets  

---

## Feature Highlights

| Feature | Description |
|--------|-------------|
| Multivariable Costing | Elevation, terrain type, and scenery included |
| Scenic Preference | Encourages routes near viewpoints |
| Elevation-Aware Routing | Avoids steep climbs when chosen |
| Obstacle Handling | Water and impassable regions avoided |
| User Customization | Prioritize distance vs. comfort vs. scenery |

---

## Experimental Results

Three controlled experiments demonstrate adaptive behavior:

### 1️⃣ Varied Terrain Types
- Trails preferred
- Efficient detours around water and obstacles

### 2️⃣ Elevation Weight Tuning
- High elevation weight → Longer but easier climbs  
- Low elevation weight → Shortest but steeper paths

### 3️⃣ Scenic Preference
- Higher scenic value → Longer scenic detours  
- Lower value → Minimal deviation from shortest path

These experiments show that A* dynamically adapts routing based on user preferences.

## Requirements
---
Python 3.x
NumPy
Matplotlib
PriorityQueue / heapq



![Path_finding](https://github.com/Bhumika0608/A-Star-Hiking-Trail-Navigator/blob/main/UI_Hiking.png)
