# Tree Search Traversal Analysis (DFS & BFS) 🌳🔍

[![Language: PT-BR](https://img.shields.io/badge/Language-PT--BR-lightgrey?style=flat-square&logo=gengo&logoColor=white)](README.pt-br.md) [![Language: PT-PT](https://img.shields.io/badge/Language-PT--PT-lightgrey?style=flat-square&logo=gengo&logoColor=white)](README.pt-pt.md)

[![Python](https://img.shields.io/badge/Python-3.10--3.11-blue?style=for-the-badge&logo=python&logoColor=white)](https://python.org) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge&logo=mit&logoColor=white)](https://opensource.org)

An educational and technical implementation of graph traversal algorithms applied to tree structures. This project analyzes and visualizes the behavioral and structural differences between **Depth-First Search (DFS)** and **Breadth-First Search (BFS)** using custom Python modules and interactive Jupyter Notebooks.

*Note: This project was originally engineered as a collaborative laboratory asset for the **Data Mining elective course (Disciplina Optativa)**, part of the **Bachelor's Degree in Computer Engineering** curriculum at the **Universidade Federal do Pará (UFPA) - Campus Tucuruí** (Academic Term: Mar 23 – Jul 23, 2026). While institutional baseline evaluation restrictions required the original repository framework and core codebase to remain unalterable in Portuguese (Brazil) during the active semester, this repository is currently undergoing an active, independent post-curriculum modernization lifecycle to transition documentation, features, and future codebase rollouts into English for international deployment and portfolio visibility.*

## 🎯 Key Objectives
- **Data Modeling:** Implement abstract tree structures utilizing adjacency lists.
- **Algorithm Analysis:** Evaluate the efficiency, pathing behavior, and memory mechanics of DFS vs. BFS.
- **Data Visualization:** Leverage graph networks to generate and export dynamic, step-by-step visual pathways of search executions.

## 🏗️ Technical Highlights & Applied Engineering
The implementation demonstrates solid foundations in software engineering and computational logic, highlighting professional practices applicable to real-world data pipelines:
- **Decoupled Architecture:** Clean separation of concerns between the core logical processing engine (`algoritmos_de_busca.py`) and the interactive test environment (`analise_comparativa_dfs_bfs.ipynb`).
- **Automated Environment Provisioning:** Built-in runtime protection block using pythonic exception handling (`try/except`) to automatically manage package setups (`networkx` and `matplotlib`) in fresh environments.
- **Time Complexity Optimization:** Utilization of specialized data structures (`collections.deque`) ensuring O(1) flat computational cost during index mutations in the BFS queue, avoiding expensive array operations.
- **Cross-Platform Host Portability:** Dynamic OS file routing abstractions (`os.path.abspath`), avoiding hardcoded structures to run seamlessly across heterogeneous environments (Unix/Windows).
- **High-Resolution Data Pipelines:** Automated analytical log extraction engine rendering high-fidelity visualizations (300 DPI exports styled with custom `monospace` alignment metrics).
- **Production Entry-Point Pattern:** Structured implementation of the `if __name__ == "__main__"` paradigm, protecting global execution namespaces and allowing isolated local unit testing without side effects upon module importation.

## 📊 Core Concepts Implemented

### 1. Depth-First Search (DFS)
* **Strategy:** Exhaustive Vertical Traversal.
* **Behavior:** Prioritizes tracking down to the leaf nodes (deepest branch) before executing backtracks to explore adjacent paths.
* **Tech Context:** Implemented recursively with explicit base-case states (`if visitados is None`) to demonstrate recursive call-stack propagation and state tracking. Time Complexity: \(\mathcal{O}(V + E)\).

### 2. Breadth-First Search (BFS)
* **Strategy:** Layer-by-Layer Horizontal Traversal.
* **Behavior:** Explores all nodes layer-by-layer (level-by-level) before descending down the hierarchy.
* **Tech Context:** Implemented using performance queue mechanics (`popleft()`), serving as the computational benchmark for finding the shortest path in terms of tree levels. Time Complexity: \(\mathcal{O}(V + E)\).

## 📸 Technical Visualization

The framework dynamically maps structural topologies and automatically exports search pathway analysis outputs into visual graph charts:

![Modelled Tree Graph Map](output/figures/mapa_da_arvore_modelada.png)

*The engine automatically verifies environments, handles conditional dynamic visual layers (#e74c3c for active targets, #2ecc71 for successful paths, and #3498db for inactive topologies), and exports logs as raw vector mapping configurations.*

## 📂 Project Architecture

```text
├── output/figures/              # Automatically generated visual outputs & high-res graphs
├── .gitignore                   # Optimized file exclusions for Python environments
├── LICENSE                      # MIT Open Source License
├── README.md                    # Main documentation (English)
├── README.pt-br.md              # Localization documentation (Portuguese - Brazil)
├── README.pt-pt.md              # Localization documentation (Portuguese - Portugal)
├── algoritmos_de_busca.py       # Core decoupled logical engines & visual mapping wrappers
└── analise_comparativa_dfs_bfs.ipynb  # Interactive analytical test bench & pipeline runner
```

## 🛠️ Tech Stack & Dependencies
- **Core:** Python 3 (OOP concepts, snake_case naming conventions matching PEP 8 style guides, and nested conditional ternary logic for in-line graph rendering).
- **Network Architecture:** `NetworkX` (for logical directed graph building, nodes parsing, and topological layout management).
- **Data Visualization Engine:** `Matplotlib` (for multi-panel subplots tracking using concurrent `zip()` loop patterns, graphic rendering, and UI export blocks).

## 🚀 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/prfs91/mapa-da-arvore-dfs-bfs.git
   cd mapa-da-arvore-dfs-bfs
   ```

2. **Run the Interactive Analysis:**
   Ensure you have Jupyter installed, or open the project folder in VS Code / Google Colab, and execute the `analise_comparativa_dfs_bfs.ipynb` notebook. The script will automatically check and install `networkx` and `matplotlib` if required.

## 👩‍💻 Authorship & Academic Context
Developed cooperatively by **Group 03** for the Data Mining elective course (UFPA):
- **Pamella Roberta** - [@prfs91](https://github.com/prfs91)
- Manuela Ferreira
- Rafaela Pinto
- Gabriel Batista

Academic Advisor: **Dr. Iago Medeiros**

---

*Actively sourcing remote software engineering opportunities, part-time contracts, or internships. Let's connect on [LinkedIn](https://www.linkedin.com/in/robertaferreira91/).*
