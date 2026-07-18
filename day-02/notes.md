# Day 2 Notes

## Commands Used

```bash
source /root/code/ml-env/bin/activate

mkdir -p /root/notebooks

/root/code/ml-env/bin/jupyter lab --config /root/code/jupyter_lab_config.py
```

## Configuration

```python
c.ServerApp.ip = "0.0.0.0"
c.ServerApp.port = 8888
c.ServerApp.root_dir = "/root/notebooks"
```

## What I Learned

- How to troubleshoot a JupyterLab configuration.
- The purpose of `ServerApp.ip`.
- Why JupyterLab needs a notebook root directory.
- How to start JupyterLab using a custom configuration file.