<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=042F2E,0F766E,2DD4BF&height=220&section=header&text=Algorithmic%20Recursion%20Suite&fontSize=40&fontColor=ffffff&fontAlignY=38&desc=Divide-and-Conquer%20Paradigms%2C%20Call-Stack%20Tracing%20and%20Complexity%20Analysis&descSize=16&descAlignY=60&descAlign=50" width="100%" alt="Algorithmic Recursion Suite Banner"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Paradigm-Recursion-042F2E?style=for-the-badge" alt="Paradigm Recursion"/>
  <img src="https://img.shields.io/badge/Language-Python%203.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Language Python 3.10+"/>
  <img src="https://img.shields.io/badge/Domain-Data%20Structures%20%26%20Algos-0F766E?style=for-the-badge" alt="Domain Data Structures & Algos"/>
  <img src="https://img.shields.io/badge/Status-Verified-10B981?style=for-the-badge" alt="Status Verified"/>
  <img src="https://img.shields.io/badge/License-MIT-2DD4BF?style=for-the-badge" alt="License MIT"/>
</p>

---

## Executive Summary / Overview
### Problem Statement & Context
Recursive formulations offer elegant, mathematically provable solutions to divide-and-conquer problems. However, an unverified base case or uncontrolled call depth easily results in stack overflows or exponential time explosion (O(2^n)). Rigorous analysis of recursive tree branching is vital for ensuring algorithmic correctness and space bounded execution.

### Solution Overview
This repository contains a dedicated academic suite analyzing **Recursive Problem Solving** in Python. Spanning two detailed notebooks (`Recursion(1).ipynb` and `Recursion.HW.ipynb`), the code demonstrates exact termination conditions, recursive state accumulation, subproblem reduction, and call-stack unwinding mechanics across a broad variety of numerical and sequence algorithms.

---

## Interactive Table of Contents
- [Executive Summary / Overview](#executive-summary--overview)
- [Key Features & Capabilities](#key-features--capabilities)
- [System Architecture / Pipeline](#system-architecture--pipeline)
- [Tech Stack Breakdown](#tech-stack-breakdown)
- [Reproducible Quickstart & Setup](#reproducible-quickstart--setup)
- [Project Directory Layout](#project-directory-layout)
- [Author & Contributions](#author--contributions)

---

## Key Features & Capabilities
- **Strict Base-Case Enforcement:** Clear boundary conditionals to prevent runaway recursion and call-stack exhaustion.
- **Divide-and-Conquer Formulations:** Practical decomposition of complex computations into self-similar sub-problems.
- **Call-Stack Visual Tracing:** Stepwise notebook cells mapping each activation record and returned accumulator value.
- **Recurrence Relation Analysis:** Explores recurrence relations and algorithmic reduction steps (e.g., T(n) = T(n-1) + O(1)).

---

## System Architecture / Pipeline
```mermaid
flowchart TD
    CallN["Recurse: func(n)"] --> BaseCheck{"Base Case Check (n <= 1?)"}
    BaseCheck -- False --> Split["Decompose: n * func(n - 1)"]
    Split --> CallN1["Recurse: func(n - 1)"]
    CallN1 --> BaseCheck2{"Base Case Check (n - 1 <= 1?)"}
    BaseCheck2 -- True --> BaseReturn["Return Base Value (1)"]
    BaseReturn --> Unwind["Unwind Stack & Multiply"]
    Unwind --> Final["Return Final Result"]
```

---

## Tech Stack Breakdown
| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Languages** | Python 3.10+ | Algorithmic scripting and execution |
| **Libraries** | Python Standard Library | Recursion limit management and stack assertions |
| **Tools** | Jupyter Notebook | Interactive cell evaluation and test-case execution |
| **Architecture** | Divide-and-Conquer Recursion | Stack frame allocation and reduction mechanics |

---

## Reproducible Quickstart & Setup
```bash
# 1. Clone repository
git clone https://github.com/suryateja-155/DSA-assignment.git
cd DSA-assignment

# 2. Virtual environment setup
python -m venv venv
.\venv\Scripts\activate   # On Windows

# 3. Install Jupyter
pip install notebook

# 4. Launch recursion lab
jupyter notebook "Recursion(1).ipynb"
```

---

## Project Directory Layout
```text
DSA-assignment/
├── Recursion(1).ipynb     # Core recursive functions and state transitions (20 cells)
├── Recursion.HW.ipynb    # Extended recursion homework and algorithmic problems (13 cells)
└── README.md             # System documentation and recurrence relation guide
```

---

## Author & Contributions

**Gettupalli Surya Teja**  
- GitHub Profile: [@suryateja-155](https://github.com/suryateja-155)  
- Portfolio Index: [Gettupalli-Surya-Teja](https://github.com/suryateja-155/Gettupalli-Surya-Teja)

Contributions, issue reports, and feedback are always welcome! Feel free to open an issue or pull request.

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=042F2E,0F766E,2DD4BF&height=100&section=footer" width="100%" alt="Footer Banner"/>
</p>
