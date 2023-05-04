Data Science Project Template
==============================

Minimal template repository for Data Science Projects.

__Instructions:__
- Fork this repo.
- Rename the `src` directory to the name you wish to give to this project's python package 
- Run a "search and replace all" over the entire project from `src` to the python package name chosen (make sure setup.py was updated).
- Rename the environment name from "dev" to the desired name in the `environment.yml` file
- Go through the installation section below to create an appropriate environment with all the necessary python dependencies installed.
- Replace this section and the title with something minigful to your project.


# Installation
Install the [conda](https://docs.conda.io/en/latest/miniconda.html) environment by running: 
```commandline
conda env create -f environment.yml
```

alternatively if you wish to update an existing one simply run 
```commandline
conda env update --file environment.yml --prune
```


## Usage
### Running the data processing pipeline
```commandline
python -m src.data.make_dataset
```
...

# Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── environment.yml    <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `conda env export --from-history > environment.yml`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    └── src                <- Source code for use in this project.
        ├── __init__.py    <- Makes src a Python module
        │
        ├── utils           <- Project wide utility code
        │   └── configs.py
        │
        ├── data           <- Scripts to download or generate data
        │   └── make_dataset.py
        │
        ├── features       <- Scripts to turn raw data into features for modeling
        │   └── build_features.py
        │
        ├── models         <- Scripts to train models and then use trained models to make
        │   │                 predictions
        │   ├── predict_model.py
        │   └── train_model.py
        │
        └── visualization  <- Scripts to create exploratory and results oriented visualizations
            └── visualize.py

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
