# Goal Tree Solver

![planning](https://img.shields.io/badge/planning-blue?style=flat-square) ![reasoning](https://img.shields.io/badge/reasoning-blue?style=flat-square) ![deer-flow](https://img.shields.io/badge/deer--flow-blue?style=flat-square)

A long-horizon planner that breaks complex objectives into verifiable dependency trees.

## Overview
Goal Tree Solver is a Python-based reasoning framework designed to tackle high-level objectives by decomposing them into structured, executable sub-tasks. By mapping dependencies within a hierarchical tree, the solver ensures that long-horizon goals are approached logically, maintaining state consistency and verifiability at every node.

## Features
*   **Hierarchical Decomposition:** Automatically breaks down complex prompts into a multi-layered dependency tree.
*   **Verifiable Logic:** Each sub-goal includes validation criteria to ensure prerequisite tasks are completed successfully.
*   **Dynamic Re-planning:** Adjusts the tree structure in real-time based on the success or failure of branch execution.
*   **Deer-Flow Integration:** Optimized for seamless workflow orchestration within reasoning-heavy environments.

## Installation
Ensure you have Python 3.8+ installed. Clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/username/goal-tree-solver.git
cd goal-tree-solver
pip install -r requirements.txt
```

## Usage
To initiate the solver, pass your primary objective to `main.py`. The system will generate a goal tree and begin processing the nodes.

```bash
python main.py --goal "Build a comprehensive market analysis report for renewable energy"
```

**Example Snippet:**
```python
from goal_solver import TreePlanner

planner = TreePlanner()
plan = planner.create_plan("Launch a beta software product")
plan.execute()
```

## Contributing
Contributions are welcome! Please submit a Pull Request or open an Issue to discuss proposed changes. Ensure all new code adheres to the existing style guidelines and includes appropriate test coverage.

## License
This project is licensed under the [MIT License](LICENSE).