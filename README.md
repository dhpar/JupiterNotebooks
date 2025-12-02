# Jupyter-Python-Practice

Personal Jupyter notebooks project for learning and practicing Python. Use this repository to experiment, take notes, and build small data-science or scripting exercises.

## Project goals
- Practice Python fundamentals and libraries.
- Try data analysis, visualization, and small ML experiments.
- Keep experiments organized and reproducible.

## Recommended environment
- Python 3.9+ (3.10/3.11 recommended)
- Use a virtual environment (venv or conda)
- Jupyter Lab or Notebook

## Quick setup (venv + pip):

1. Create and activate a virtual environment
- macOS / Linux:
```bash
python3 -m venv .venv
source .venv/bin/activate
```
- Windows (PowerShell):
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Upgrade pip and install core dependencies
```bash
pip install --upgrade pip
pip install jupyterlab ipykernel numpy pandas matplotlib seaborn scikit-learn
```

3. Register an IPython kernel for this project
```bash
python -m ipykernel install --user --name jupyter-python-practice --display-name "Jupyter-Python-Practice"
```

4. Start Jupyter
```bash
jupyter lab
```

5. Record or install pinned dependencies
- Save current environment:
```bash
pip freeze > requirements.txt
```
- Recreate from requirements:
```bash
pip install -r requirements.txt
```

6. Helpful repository notes
- Add common entries to .gitignore: .venv/, __pycache__/, .ipynb_checkpoints/
- Keep notebooks small and include a requirements.txt or environment.yml for reproducibility.

Optional: Conda alternative
```bash
conda create -n jpprac python=3.11 -y
conda activate jpprac
conda install -c conda-forge jupyterlab ipykernel numpy pandas matplotlib seaborn scikit-learn
python -m ipykernel install --user --name jupyter-python-practice --display-name "Jupyter-Python-Practice"
```