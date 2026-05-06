# DM2026 Assignment 2
112550191 許書瑋
This repository contains the code, notebooks, figures, and LaTeX report for Assignment 2.

## Project Structure

- `Mobile_Price_Sections.ipynb`: Sections 2--5 for the mobile price dataset.
- `Real_World_Classification.ipynb`: Section 1 cross-validation/classification work.
- `model/`: custom model, gradient, metric, and utility code used by the notebooks.
- `data/`: input datasets.
- `pics/`: figures used by `report.tex`.
- `report.tex`: LaTeX source for the final report.
- `DM_asg2_112550191.pdf`: generated report PDF.

## Environment Setup

Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the Python packages used by the notebooks:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy mlxtend ipython jupyter graphviz
```

The `graphviz` Python package may also require the system Graphviz executable if tree visualizations are regenerated:

```bash
sudo apt-get install graphviz
```

## Run the Notebooks

Start Jupyter from the repository root:

```bash
jupyter notebook
```

Then run:

1. `Real_World_Classification.ipynb`
2. `Mobile_Price_Sections.ipynb`

Run cells from top to bottom so that intermediate variables and generated figures are available.

## Build the Report

The report uses the figures in `pics/`, so build it from the repository root:

```bash
pdflatex report.tex
pdflatex report.tex
```

If `pdflatex` is not installed, install a TeX distribution such as TeX Live, or upload the project to Overleaf and compile `report.tex` there.

The expected output is `report.pdf`. The submitted PDF in this repository is `DM_asg2_112550191.pdf`.

