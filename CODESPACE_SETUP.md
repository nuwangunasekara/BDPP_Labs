# Setting Up a GitHub Codespace

This guide explains how to set up a GitHub Codespace for this project using `.devcontainer.json`, `requirements.txt`, and `.gitignore`.

## Prerequisites

1. Ensure you have access to GitHub Codespaces.
2. A repository containing the following files:
   - `.devcontainer/devcontainer.json`
   - `requirements.txt`
   - `.gitignore`

---

## Steps to Set Up the Codespace

### Add `devcontainer.json`
Create a `.devcontainer.json` file with the following content:

```json
{
    "name": "Python and Java Dev Environment",
    "image": "mcr.microsoft.com/devcontainers/python:3.8",
    "features": {
        "ghcr.io/devcontainers/features/conda:1": {
            "version": "latest"
        },
        "ghcr.io/devcontainers/features/java:1": {
            "version": "17"
        }
    },
    "customizations": {
        "vscode": {
            "extensions": [
                "ms-python.python",
                "ms-toolsai.jupyter",
                "redhat.java"
            ]
        }
    },
    "postCreateCommand": "pip install -r requirements.txt"
}
```

### Add `requirements.txt`
```
pyspark
pandas
pyarrow
notebook
```

### Add `.gitignore`
```
__pycache__/
*.pyc
*.pyo
*.ipynb_checkpoints/
.env/
```


