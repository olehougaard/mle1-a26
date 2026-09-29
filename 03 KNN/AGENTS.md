# AGENTS.md

## Project context

This workspace is a small educational machine-learning project focused on K-Nearest Neighbors (KNN), built mainly as Jupyter notebooks rather than a packaged application.

Primary files:
- `basics.ipynb` — Python and notebook basics
- `matrix.ipynb` — matrix/vector examples
- `visualizations_knn.ipynb` — decision boundaries and visualization examples
- `digit_mnist.ipynb` — digit classification with scikit-learn
- `fashion_mnist.ipynb` — fashion image classification using KNN
- `Titanic.csv` and `temp_energy.csv` — local datasets used in notebooks

## Working conventions

- Treat this as a notebook-first project. Changes are usually made inside notebook cells, not in a separate src package.
- Prefer Python + NumPy + pandas + scikit-learn patterns already used in the notebooks.
- Keep code cell execution order and imports explicit; avoid hidden state between cells.
- Use relative data paths such as `./Titanic.csv` or `./temp_energy.csv` when a notebook is run from the workspace root.
- Preserve educational clarity: code should be readable, small, and easy to follow.

## Validation guidance

- There is no formal test suite or package build in this repo.
- Validate changes with the smallest relevant Python execution or notebook cell run.
- For KNN-related edits, check the actual output of the model fit/score step rather than relying only on import success.
- Prefer focused sanity checks over broad project-wide execution.

## Avoid

- Creating a full application structure when the project is clearly notebook-based.
- Adding complex tooling or dependencies unless a notebook explicitly requires them.
- Rewriting notebook logic into unrelated frameworks or custom abstractions.
- Assuming there are hidden source files or a package entry point when the repo is primarily notebooks.

## When helping with this repo

- Keep answers aligned with an educational ML context.
- Explain KNN concepts simply when code is being modified or debugged.
- If a notebook example is changed, maintain consistency with the existing sklearn usage and plotting style.
