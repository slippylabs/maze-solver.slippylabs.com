# Maze Generator & Pathfinder

Generate mazes and watch BFS, Dijkstra, A* and greedy best-first search solve them step by step, with visited-order heatmaps and live node counts.

**Live:** <https://maze-solver.slippylabs.com/>

## What it does

- Generate a maze with a recursive backtracker or randomised Prim's.
- Race breadth-first search, Dijkstra, A* (Manhattan heuristic) and greedy best-first through it.
- Watch them crawl a step at a time, with visited-order heatmaps and live node counts.
- Draw your own walls and paint terrain costs to see where the heuristics break down.

## How it works

Running the four searches over the same grid makes the difference between them visible rather than theoretical: greedy best-first charges at the goal and takes a bad route, BFS floods evenly and finds the shortest path in the unweighted case, Dijkstra respects terrain cost, and A* does the same work as Dijkstra but visits far fewer nodes. The visited-order heatmap is where that shows up.

## Run it locally

A static site. No build step, no package manager, no dependencies:

```
git clone git@github.com:slippylabs/maze-solver.slippylabs.com.git
cd maze-solver.slippylabs.com
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

---

Part of [Slippy Labs](https://slippylabs.com). Every tool is indexed at
[projects.slippylabs.com](https://projects.slippylabs.com).
