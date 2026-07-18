# Day 01: Python Environment Architecture

## Overview
Foundation day focused on initializing isolated development workspaces and structuring reproducible dependency tracking. This documentation covers both traditional Python tooling and modern, high-velocity `uv` workflows.

---

## Tool Comparison: Why `uv` is Better

| Metric | Traditional Python Tooling | Modern MLOps Tooling (`uv`) |
| :--- | :--- | :--- |
| **Speed** | Slow (Sequential downloads) | Ultra-fast (Parallel Rust engine) |
| **Command** | `python3 -m venv` & `pip install` | `uv venv` & `uv pip install` |
| **Caching** | Global but basic | Aggressive, global content-addressable cache |

---

## Production Execution Logs

### Method A: Modern `uv` Workflow (Recommended)
```bash
# Ensure target deployment workspace exists
mkdir -p /root/code && cd /root/code/

# Provision isolated environment with uv instantly
uv venv ml-env --python 3.11

# Activate runtime instance boundaries
source ml-env/bin/activate

# Execute ultra-fast parallel package injection
uv pip install numpy pandas scikit-learn matplotlib

# Compile a cryptographically locked requirements file
uv pip compile -o requirements.txt
```

### Method B: Traditional Baseline Workflow
```bash
# Provision isolated standard environment
python3 -m venv ml-env
source ml-env/bin/activate

# Install packages sequentially
pip install numpy pandas scikit-learn matplotlib

# Freeze loose dependency list
pip freeze > requirements.txt
```

---

## Artifact Verification
* **Environment Status**: Isolated virtual environment activated successfully.
* **Lock State**: `requirements.txt` correctly compiled with precise dependency mappings.
