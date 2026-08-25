# Environment setup

The course uses [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) and
a Python kernel named **Python (MATH 465)**. JupyterLab is recommended,
although the classic Jupyter Notebook can also run the course `.ipynb` files.

## Recommended: Conda

These instructions work on macOS, Windows, and Linux.

### 1. Confirm that Conda is installed

Open a terminal and run:

```bash
conda --version
```

If this prints a version number, continue below. If Conda is not installed,
[Miniforge](https://github.com/conda-forge/miniforge) is one way to install it.

### 2. Download the course files

Clone the repository and enter its folder:

```bash
git clone https://github.com/xycheng/math465_f2026.git
cd math465_f2026
```

If you do not use Git, select **Code > Download ZIP** on GitHub, extract the
file, and open a terminal in the extracted folder.

### 3. Install the environment and kernel

```bash
conda env create -f environment.yml
conda activate math465
python -m ipykernel install --user --name math465 --display-name "Python (MATH 465)"
```

### 4. Start JupyterLab

```bash
python -m jupyter lab
```

Open a course notebook and select the **Python (MATH 465)** kernel.

## Alternative: Python and pip

Use this option if Python 3.11 is already installed.

### macOS or Linux

```bash
python3.11 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m ipykernel install --user --name math465 --display-name "Python (MATH 465)"
python -m jupyter lab
```

### Windows PowerShell

```powershell
py -3.11 -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m ipykernel install --user --name math465 --display-name "Python (MATH 465)"
python -m jupyter lab
```

In JupyterLab, open a course notebook and select the **Python (MATH 465)**
kernel.
