# Day 3 - Managing Python Dependencies with uv

## Objective

Learn how to manage Python project dependencies using `uv` and generate a reproducible lockfile.

## Lab Scenario

A project contained an incorrect `requirements.in` file. The task was to correct the dependency specification and compile a pinned `requirements.txt` lockfile using `uv`.

## Requirements

- Correct `requirements.in`
- Include exactly four top-level packages:
  - scikit-learn
  - mlflow
  - pandas
  - numpy
- Generate a pinned `requirements.txt` with exact versions and all transitive dependencies.

## Outcome

Successfully corrected the dependency specification and generated a reproducible lockfile using `uv`.