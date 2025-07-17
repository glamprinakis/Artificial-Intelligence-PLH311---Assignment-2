# Artificial Intelligence — PLH311  
## 2nd Programming Assignment · **TUC‑CHESS Search Agents**

This repository contains **Team 38’s** solution for the second programming assignment
of the *Artificial Intelligence (PLH311)* course.  
The task: build a competitive **search agent** for **TUC‑CHESS**—a
custom chess variant in which capturing (or simply occupying) *scoring squares*
earns points throughout the game.

---

## ✨ Project Highlights
| Component | Purpose |
|-----------|---------|
| `team38_project2/` | All Java source code (model, game logic, three AI agents). |
| `AI_project_2_2022 (TUC‑CHESS‑2022)‑Final.pdf` | Full technical report & experimental results. |
| `README.md` | *You are here.* |

### Implemented AI Algorithms
1. **Minimax** – classic adversarial search with depth‑limited look‑ahead.  
2. **Alpha–Beta Pruning** – Minimax + branch pruning and move ordering for speed‑ups.  
3. **Monte‑Carlo Tree Search (MCTS)** – stochastic playouts with UCB1 selection, expansion,
   simulation, and back‑propagation phases.

> All three agents share a common game‑state representation (`Move`, `Board`,
> `Agent` classes) to enable fair benchmarking. :contentReference[oaicite:0]{index=0}

---

## 📂 Quick Tour of the Code

```
├── team38_project2/
│ ├── board/ # Piece, Board, Move …
│ ├── agents/
│ │ ├── MinimaxAgent.java
│ │ ├── AlphaBetaAgent.java
│ │ └── MCTSAgent.java
│ ├── heuristics/ # Static evaluation & cutoff functions
│ └── Main.java # CLI entry‑point
├── AI_project_2_2022 (TUC-CHESS-2022)-Final.pdf
└── README.md
```
##📈 Results

Our best configuration **(Alpha‑Beta, depth = 5, heuristic = “material + positional
score”)** achieved the highest average score and the fastest decision time across
all tested time limits. Detailed tables, plots, and discussion can be found in
section 4 of the accompanying PDF report.


