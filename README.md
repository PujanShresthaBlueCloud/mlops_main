mlops_main
==============================

its a wafer project using mlops

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
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
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

# git hub link for the code
https://github.com/c17hawke/mlops_main/tree/main

for setup 
https://c17hawke.github.io/wafer_mlops_docs/stage1_init_setup/

# google api console for dvc authentication
https://console.cloud.google.com/apis/credentials/consent?project=mlopsend2end&supportedpurview=project

For google setup
https://dvc.org/doc/user-guide/data-management/remote-storage/google-drive#google-drive

Add remote storage we have created mlops_end_to_end_data floder in google drive inside MyDrive
dvc remote add -d storage gdrive://<DRIVE ID>
dvc remote add -d storage gdrive://1pxN01xa2zjzpSCRlQyVwg1wCzha4rSjC

dvc remote modify storage gdrive_client_id '68158427861-6ahul0l6mjdfhpcs68efg7uliv6ojl8o.apps.googleusercontent.com'
dvc remote modify storage gdrive_client_secret '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'

git add .dvc/config && git commit -m "Configure remote storage"
