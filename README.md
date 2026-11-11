# DS 218 Final Requirement — Personality Classification

This repository contains a Jupyter Notebook for a data science project that explores social-media behavior features and classifies users as introverted (`0`) or extroverted (`1`).

## Project workflow

The notebook covers:

1. **Data understanding** — identifies the target variable and the numerical and categorical features.
2. **Preprocessing** — checks missing values and outliers, applies one-hot encoding, and standardizes numerical features.
3. **Dimensionality reduction** — uses Principal Component Analysis (PCA) and t-distributed Stochastic Neighbor Embedding (t-SNE) for analysis and visualization.
4. **Classifier selection** — compares Logistic Regression, k-Nearest Neighbors, Decision Tree, and Random Forest.
5. **Training and tuning** — uses an 80/20 train-test split and `GridSearchCV` for hyperparameter tuning.
6. **Evaluation** — reports classification metrics and displays confusion-matrix visualizations.
7. **Interpretation and reflection** — discusses findings, limitations, and possible improvements.

## Repository contents

| File | Description |
| --- | --- |
| `DS218_Final_Requirement_GitHub.ipynb` | Formatted project notebook with saved outputs and graph images. |
| `README.md` | Project overview and setup instructions. |
| `personality.csv` | **Required dataset; add this file to the repository root before rerunning the notebook.** |

> **Dataset note:** The CSV dataset was not included with the notebook provided for editing. The notebook reads it using `pd.read_csv('personality.csv')`, so the file must be named exactly `personality.csv` and placed in the same repository folder as the notebook. Only publish the dataset if you have permission to share it.

## Viewing the results on GitHub

1. Open the repository on GitHub.
2. Select `DS218_Final_Requirement_GitHub.ipynb`.
3. GitHub should display the Markdown sections, code cells, saved tables, and embedded graph outputs in notebook format.

The notebook supplied here retains its existing saved outputs, including graph images. GitHub displays those saved results; it does not execute the Python code. To reproduce the analysis, use Google Colab or a local Jupyter environment and provide the dataset described above.

## Running the notebook in Google Colab

1. Upload `personality.csv` into the Colab session's file area so it is available at the notebook's working directory.
2. Open the notebook in Colab.
3. Choose **Runtime → Run all**.
4. After the notebook finishes, choose **File → Download → Download .ipynb** to save the notebook with its latest outputs.
5. Upload the downloaded notebook to the repository if you want GitHub to show the newly generated results.

## Python libraries

The notebook imports the following main libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Google Colab already includes these common data-science libraries in many runtimes. In a local Python environment, install them with:

```bash
python -m pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Uploading or replacing the notebook on GitHub

1. Open your GitHub repository.
2. Select **Add file → Upload files**.
3. Drag in `DS218_Final_Requirement_GitHub.ipynb` and `README.md`.
4. Make sure the notebook is uploaded to the repository's main folder (the same folder where you will place `personality.csv`).
5. Enter a commit message such as `Add formatted DS218 project notebook and README`.
6. Select **Commit changes**.

If your repository already contains the original notebook, use the same destination path and filename when replacing it, or remove the old notebook after confirming that the new file is committed. Avoid uploading a `.py` export in place of the `.ipynb` file: the `.ipynb` format preserves separate Markdown, code, and output cells.
