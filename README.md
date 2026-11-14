# DSCI 552 Homework 7

Hongwei Xiao (Ga9a)

The executed notebook is `notebooks/Xiao_Hongwei_HW7.ipynb`. It contains the code, outputs, explanations, and ISLR 12.6.2 answers. `Xiao_Hongwei_HW7.pdf` is the printable copy.

## Run

Use Python 3.12 and install the dependencies:

```sh
python -m pip install -r requirements.txt
```

Open the notebook and run the cells in order. Keep `data/`, `notebooks/`, and `results/` in the same directory. The notebook works when started from either the repository root or `notebooks/`.

Question 1 uses a fixed 70/30 split and 10-fold cross-validation for each target. It compares RBF SVM, L1 linear SVM, and L1 linear SVM with balanced class weights. Scaling is fitted within the training folds. Question 2 repeats K-means 50 times on the full dataset, selecting k independently in each run by the Calinski-Harabasz score. Each candidate uses 10 initializations. Rerunning takes several minutes or longer, depending on the machine; six parallel workers are used.

## Files

- `data/`: the original Anuran Calls CSV and dataset description.
- `notebooks/`: the executed notebook.
- `results/`: cross-validation tables, predictions, selected cluster labels, all 50 runs, summary statistics, and figures.
- `requirements.txt`: package versions used.
- `Xiao_Hongwei_HW7.pdf`: notebook with code and saved results.

The extra-practice questions are not included. The dataset comes from the [UCI Anuran Calls repository](https://archive.ics.uci.edu/dataset/406/anuran+calls+mfccs).
