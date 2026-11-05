# MATH 465: High-Dimensional Data Analysis

Python demonstrations for MATH 465, Fall 2026.

## Quick start

The course uses [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/).
For instructions on installing Conda and JupyterLab, see
[Environment setup](SETUP.md). The classic Jupyter Notebook can also run the
course `.ipynb` files, but JupyterLab is recommended.

With Git and Conda installed, run the following commands in a terminal:

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

If a code cell shows `[*]`, it is running or waiting to run. A number such as
`[1]` is its execution count: it records the order in which code cells were
run, rather than their position in the notebook. Check the output for any
error messages.

## Demos

| Module | Demo |
| --- | --- |
| 1 | [Setup, computational scaling, and random seeds](demos/Module1_setup_plots_seed.ipynb) |
| 1 | [k-means](demos/Module1_kmeans.ipynb) |
| 2 | [Demo 1: Basic PCA on simulated and Wine data](demos/Module2_PCA1.ipynb) |
| 2 | [Demo 2: PCA of evolving data and high-dimensional images](demos/Module2_PCA2.ipynb) |
| 2 | [Demo 3: PCA when the dimension exceeds the sample size](demos/Module2_PCA3.ipynb) |
| 3 | [Demo 1: MDS and Isomap](demos/Module3_MDS_Isomap.ipynb) |
| 3 | [Demo 2: t-SNE on clustered data and the Swiss roll](demos/Module3_tSNE.ipynb) |
| 4 | [Spectral clustering](demos/Module4_spectral_clustering.ipynb) |
| 5 | [Random matrices and random graphs](demos/Module5_random_matrices_graphs.ipynb) |

Additional demonstrations will be added during the semester.

## Updating the course files

From a terminal inside the `math465_f2026` repository folder, run:

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
