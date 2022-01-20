# Cookiecutter Data Science

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._




#### [Project homepage](http://drivendata.github.io/cookiecutter-data-science/)


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5+
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter  https://github.com/faviasono/cookiecutter-data-science


[![asciicast](https://asciinema.org/a/244658.svg)](https://asciinema.org/a/244658)


### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── .azureml     
│      └── config.json <- Add AzureML workspace information        
│
├── data              
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump: Use .CSV/txt format to map 
│        │                 names to files in Cloud storage.                   
│        └── README.md <- Describe data you will use in your project.   
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries: store initial models
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│   ├                      the creator's initials, and a short `-` delimited description, e.g.
│   ├                     `1.0-jqp-initial-data-exploration`.
│   ├── development      <- Initial experiments 
│   ├── azureml_pipeline <- Creating the azureml pipeline in this folder to submit jobs
│   ├── README.md        <- Describe experiments in high-level (and provide reference in notebooks)
│
├── references         <- Data dictionaries, research papers, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
├── src                <- Source code for use in this project: it will be used during the creation of the pipeline for AzureML.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   ├── build_features.py
│   │   └──README.md   <- Describe the preprocessing steps at high-level. Add the WHY to the description.
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   ├── train_model.py
│   │   └──README.md   <- Describe the molde used at high-level. Add the WHY to the description.
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io
```


### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests

### Code Formatter
------------
Black is the uncompromising Python code formatter. Use black to reformat your repo according to the PEP8 guidelines.\
Github page [here](https://github.com/psf/black).


    pip install black
    pip install black[jupyter]
    black {source_file_or_directory}


## Extra resources for coding

### [The seven rules of a great Git commit message](https://heady-booth-f73.notion.site/The-seven-rules-of-a-great-Git-commit-message-acd037698a574974b9b18edb6f72960d): how to write effective and useful git commits for collaboration

### [Mypy - Python Type Hints](https://heady-booth-f73.notion.site/Typing-ffa6a8b1f824451ca7d9542ef3030fcf): using Python type hints to quick test code


### [Toxi](https://tox.readthedocs.io): automate and standardize testing in Python

### [Sphinx ](https://www.sphinx-doc.org/en/master/): intelligent and beautiful documentation
