##  Developer notes
- Every Part of the pillar contains their own readme files containing the questions of the topic.

# 🛠️ Local Setup Guide

> For running the notebooks in this repo on your local machine using Cursor (or any VS Code-based editor).

---

## Prerequisites

- Python 3.10+ installed (`python --version` to check)
- Cursor (or VS Code) with the Jupyter extension

> **Note on Python version:** This repo was set up and tested with **Python 3.12.7**. If you hit install errors, your Python version may be the culprit — some packages have minimum version requirements. Check with `python --version` before proceeding, and consider upgrading if you're on anything below 3.10.

---

## Setup Steps

### 1. Clone the repo

```bash
git clone <repo-url>
cd AIM-Pillar-3-Required-Assignment
```

### 2. Create a virtual environment

> ⚠️ **We are NOT using `uv` here.** Plain `venv` + `pip` is simpler and sufficient for this assignment notebook. No `pyproject.toml` or `uv.lock` needed.

```bash
python -m venv .venv
```

### 3. Activate it

```bash
# Mac/Linux
source .venv/bin/activate

# Windows
.venv\Scripts\activate
```

You should see `(.venv)` at the start of your terminal prompt.

### 4. Install dependencies

```bash
pip install ipykernel numpy pandas matplotlib seaborn scikit-learn
```

### 5. Register the kernel with Jupyter

```bash
python -m ipykernel install --user --name=.venv --display-name "Python (.venv)"
```

This makes the `.venv` environment visible to Cursor's kernel selector.

### 6. Select the kernel in Cursor

1. Open any `.ipynb` file
2. Click **Select Kernel** (top-right corner)
3. Choose **Python Environments** → **Python (.venv)**
4. Hit **Run All**

---

## Important: Add `.venv` to `.gitignore`

The `.venv` folder should **never** be committed to the repo. If you don't have a `.gitignore` yet:

```bash
echo ".venv/" >> .gitignore
```

This prevents thousands of virtual environment files from showing up as untracked changes in Git.

---

## Datasets

Make sure the required CSV files are inside the `datasets/` folder before running the notebooks. For example:

- `datasets/Mall_Customers.csv` — used by `task1_kmeans.ipynb`

These are not installed via pip — they should already be in the repo.

---

## Why not `uv`?

`uv` is a great tool for production Python projects (faster installs, lockfiles, workspace management). But for a single notebook assignment like this, plain `venv` + `pip` is the right choice — less setup, no extra tooling required, and it works out of the box on any machine with Python installed.

Use `uv` when you're building services, APIs, or multi-package projects. Use `venv` when you just need to run a notebook.