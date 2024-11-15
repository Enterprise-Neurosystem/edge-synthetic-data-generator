# edge-synthetic-data-generator

Open source code for generation of synthetic sensor data.

## Team Members

1. Cameron Garrison
1. Christina Xu
1. Marius Bogoevici
1. Trevor Royer

## Usage

Typical usage is within a `Standard Data Science Notebook` image, with pip installs inside the notebook as needed.

However, `requirements.txt` is provided with full python packages/versions for usage (tested with python 3.9) outside of RHOAI / ODH.

## Structure

    ├── data                            # Data files used for model training and plots.
    ├── docs                            # Documentation and workshop info
    ├── models                          # A few saved, pretrained DGAN models.
    ├── notebooks                       # Initial notebooks, testing data generation methods.
    ├── 12-generate-sensor-data.ipynb   # Primary nb used to create and stream synthetic data.
    ├── LICENSE
    ├── requirements.txt                # Standard python requirements file.
    └── README.md

Note that some early notebooks in explanatory-notebooks require downloading dataset from Kaggle (linked in code) and some point to models that you must train yourself (typically in the prior notebook). These notebooks are intended to show other methods of synthetic data generation that didn't work for our use case, but may be of use for others.
