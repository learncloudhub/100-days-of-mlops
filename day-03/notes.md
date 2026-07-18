# Day 3 Notes

## Commands Used

Navigate to the project

```bash
cd /root/code/fraud-detection
```

Edit the dependency specification

```bash
vi requirements.in
```

Contents of `requirements.in`

```text
scikit-learn
mlflow
pandas
numpy
```

Compile the lockfile

```bash
uv pip compile requirements.in -o requirements.txt
```

Verify the generated file

```bash
cat requirements.txt
```

## What I Learned

- Difference between `requirements.in` and `requirements.txt`
- How `uv` resolves dependencies
- Why lockfiles improve reproducibility
- Importance of pinning package versions