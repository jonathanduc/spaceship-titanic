# Spaceship Titanic - Machine Learning Classification

An end-to-end supervised learning project based on the Kaggle **Spaceship Titanic** competition. The objective is to predict whether a passenger was transported to an alternate dimension using demographic, travel and spending information.

This project was completed during my first year of Master's studies and is kept public as part of the progression of my Data Science portfolio.

## Project overview

The work covers the main stages of a classical tabular Machine Learning workflow:

- exploratory data analysis
- missing-value handling and preprocessing
- feature engineering
- statistical modelling
- Logistic Regression, Random Forest and SVM comparison
- confusion-matrix analysis and ROC/AUC evaluation
- cross-validation
- generation of a Kaggle submission

## Results

The strongest local results observed in the final notebook include:

| Model | Accuracy | Additional metric |
| --- | ---: | --- |
| Logistic Regression | 0.784 | Sensitivity 0.822 |
| Random Forest | 0.798 | F1 0.789 |
| SVM | 0.788 | ROC AUC 0.878 |

Using the selected SVM decision threshold, the evaluation produced approximately **0.792 accuracy** and **0.794 F1** on the held-out test split.

These scores are reported from the notebook included in this repository. They are local validation results and should not be confused with a Kaggle leaderboard score.

## What I worked on

I carried out the project end to end, from exploratory analysis to the final submission workflow. Particular attention was given to:

- understanding relationships between passenger characteristics and the target
- comparing statistical and Machine Learning approaches rather than relying on a single model
- analysing sensitivity, specificity, precision and F1 in addition to accuracy
- using ROC curves and probability thresholds to study classification behaviour
- documenting the work through notebooks, reports and a presentation

## Repository structure

```text
.
├── Notebooks/
│   ├── Spaceship_two_final.ipynb
│   └── resultats/
├── Memoire/
│   ├── Presentation/
│   └── Rapports/
├── soumission/
├── requirements.txt
└── README.md
```

## Tech stack

- Python
- Pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

The main analysis is available in `Notebooks/Spaceship_two_final.ipynb`.

## What I would improve today

This is an earlier project and I deliberately keep it in my portfolio to show my progression. If I rebuilt it today, I would separate preprocessing and modelling into reusable Python modules, use a reproducible sklearn Pipeline, add automated tests, track experiments and expose the final model through a small inference service.

Those engineering practices are now part of the way I approach newer Data and ML projects.

## Author

**Jonathan Duckes**

- GitHub - https://github.com/jonathanduc
- LinkedIn - https://www.linkedin.com/in/jonathan-duckes/
- Portfolio - https://jonathanduc.github.io/portfolio/
