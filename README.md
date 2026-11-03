# Optimal Low-Rank Matrix Approximation with the SVD: Theory and Image Compression Example

The singular value decomposition (SVD) factorizes any matrix into two orthogonal matrices of singular vectors and a diagonal matrix of non-negative singular values, ordered from largest to smallest. Truncating this factorization gives the best low-rank approximation of the matrix in the Frobenius norm, a result known as the Eckart–Young theorem.

This project presents the SVD in its full, economy and truncated forms, explains its geometric meaning, and states the Eckart–Young theorem. The theory is illustrated with image compression: a full color photograph is converted to grayscale and approximated with several ranks. The decay of the singular values and their cumulative sum show how many components are needed to balance compression and quality. The article closes with other applications of the SVD and directions for further study.

The whole article is in one Jupyter notebook: [`svd-article.ipynb`](svd-article.ipynb).

## Technologies

- Python 3
- [NumPy](https://numpy.org/) for the SVD and matrix computations
- [Matplotlib](https://matplotlib.org/) for reading the image and drawing the plots
- [Jupyter Notebook](https://jupyter.org/) for the article, with math written in LaTeX

## Project structure

```
svd-explained/
├── svd-article.ipynb     # the article with the code and figures
├── data/
│   └── cat.jpg           # the photograph used in the image compression example
├── images/               # figures used in the article
└── README.md
```
## Requirements

- Python 3 (3.10 or newer is recommended)
- The packages `numpy`, `matplotlib` and `notebook`, which can be installed with:

  ```
  pip install numpy matplotlib notebook
  ```

If you use Anaconda, these packages are already installed.

## How to run

1. Download or clone this repository.
2. Open a terminal (or Anaconda Prompt) in the repository folder and start Jupyter:

   ```
   jupyter notebook
   ```

   A browser window opens with the files in the folder.
3. Click `svd-article.ipynb` to open it.
4. Run all cells from top to bottom (**Kernel → Restart & Run All**).

Other ways to open the notebook:
- **JupyterLab:** run `jupyter lab` instead (after `pip install jupyterlab`).
- **VS Code:** open the folder, open `svd-article.ipynb` and select a Python kernel (requires the Jupyter extension).
- **Anaconda Navigator:** launch Jupyter Notebook, browse to the folder and open the file.