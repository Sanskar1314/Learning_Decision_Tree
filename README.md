# Learning Decision Trees

A Jupyter notebook exploring decision tree classification on the Iris dataset.

## Contents

- `Decision_Tree_Classifier.ipynb`: loads Iris features and labels, makes an 80/20 train/test split, trains a baseline decision tree, and plots it.
- A five-fold GridSearchCV explores splitting criteria, splitter strategies, maximum depth, and feature selection.
- Evaluation includes confusion matrices, classification reports, and accuracy.

## Run locally

Use Python 3 and run Jupyter from the repository directory.

```bash
git clone https://github.com/Sanskar1314/Learning_Decision_Tree.git
cd Learning_Decision_Tree
python -m venv .venv
source .venv/bin/activate
python -m pip install jupyterlab numpy pandas matplotlib scikit-learn
jupyter lab
```

On Windows, activate the environment with `.venv\Scripts\activate`. Open the notebook listed above and run its cells in order. Results and visualizations appear in the notebook.

## Reproduction notes

Iris is available directly through scikit-learn. The search grid contains `max_features='auto'`, which is unsupported by newer scikit-learn versions; remove that candidate or replace it with `None` before tuning. The notebook is an educational experiment rather than a packaged application.
