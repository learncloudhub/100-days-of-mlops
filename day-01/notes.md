# Day 1 Notes

## Topic
Virtual Environments with uv and Python venv

## Commands Used

### Create a virtual environment with uv
```bash
uv venv ml-env --python 3.11
```

### Activate the virtual environment

**Windows (PowerShell)**
```powershell
.\ml-env\Scripts\Activate.ps1
```

**Linux/macOS**
```bash
source ml-env/bin/activate
```

### Install packages
```bash
uv pip install numpy pandas scikit-learn matplotlib
```

### Generate requirements.txt
```bash
uv pip compile -o requirements.txt
```

## What I Learned

- Why virtual environments are important.
- How `uv` can create and manage Python environments.
- How to install Python packages inside an isolated environment.
- How to generate a `requirements.txt` file for reproducible projects.

## Challenges

- Learned the difference between `uv` and the standard `venv` module.
- Practiced activating a virtual environment and managing dependencies.

## Summary

Successfully created a virtual environment, installed required packages, and generated a requirements file.