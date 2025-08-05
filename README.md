# 🛠️ pybench

A minimal local Python workbench template and setup instructions for quick local development and testing.

## Requirements

- [VSCode](https://github.com/microsoft/vscode) 
    - [VSCode Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
    - [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- [uv](https://github.com/astral-sh/uv)

## How To Setup

1. Install all requirements.

2. Clone repository.

3. Navigate to the `pybench/` folder.

4. Initialize uv project.

    ```bash
    uv init --python=3.<version_number>
    ```

5. Generate virtual environment.

    ```bash
    uv venv
    ```

6. Install ipykernel pip package to interface with VSCode Jupyter extension.

    ```bash
    uv pip install ipykernel
    ```

## How To Use

### Installing Dependencies

```bash
uv add <package_name>
```

```bash
uv pip install <package_name>
```

### Running .py Files

```bash
uv run <file_name>.py <args>
```

### Running .ipynb Notebooks

Notebooks can be run from within VSCode via the Jupyter Extension by selecting the pybench venv kernel.