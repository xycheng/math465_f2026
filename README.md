# MATH 465: High-Dimensional Data Analysis

Python demonstrations for MATH 465, Fall 2026.

## Quick start

The course uses [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/).
For instructions on installing Conda and JupyterLab, see
[Environment setup](SETUP.md). The classic Jupyter Notebook can also run the
course `.ipynb` files, but JupyterLab is recommended.

```bash
git clone https://github.com/xycheng/math465_f2026.git
cd math465_f2026
conda env create -f environment.yml
conda activate math465
python -m ipykernel install --user --name math465 --display-name "Python (MATH 465)"
python -m jupyter lab
```

In JupyterLab, select the **Python (MATH 465)** kernel.

## Using a notebook for the first time

A Jupyter notebook is an `.ipynb` file that combines text, Python code, and
the output produced by the code. A notebook is divided into cells.

1. After you run `python -m jupyter lab`, JupyterLab opens in a web browser.
2. Use the file browser on the left to find and open a course `.ipynb` file.
3. Confirm that **Python (MATH 465)** is selected as the kernel in the
   upper-right corner.
4. Click a code cell and press **Shift+Enter** to run it. Its output appears
   below the cell.
5. Cells share variables, so their order matters. To run a notebook cleanly
   from the beginning, use **Kernel > Restart Kernel and Run All Cells**.
6. Save the notebook with **File > Save Notebook**, `Ctrl+S` on Windows and
   Linux, or `Command+S` on macOS.

If a cell shows `[*]`, it is still running. A number such as `[1]` means that
the cell has finished and records its position in the execution order.

## Demos

| Module | Notebook | Topics |
| --- | --- | --- |
| 1 | [Setup, plots, random seeds](demos/Module1_setup_plots_seed.ipynb) | Environment check, computational scaling, and reproducibility |

Additional demonstrations will be added during the semester.

## Updating the course files

From inside the repository, run:

```bash
git pull
```

## Files

- `demos/`: lecture demonstration notebooks
- `environment.yml`: recommended Conda environment
- `requirements.txt`: packages for the alternative pip setup
- `SETUP.md`: environment setup instructions

Xiuyuan Cheng

xiuyuan.cheng@duke.edu
