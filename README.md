# Readme for the Housing EDA Project



## Requirements

- pyenv
- python==3.9.8
- pip

## Setup

One of the first steps when starting any data science project is to create a virtual environment. The general workflow consists of... 

* setting the python version locally to 3.9.8
* creating a virtual environment using the `venv` module
* activating your newly created environment 
* upgrading `pip` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
* installing the required packages via `pip`

If you need additional packages don't forget update your requirements.txt file.
Therefore you can create a `requirements file` and add it to your repository. You can create such a file by running the following command: 

```bash
pip freeze > requirements.txt
```

*Note: In rare case such a requirements file created with `pip freeze` might not ensure that another (especially M1 chip) user can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment variables and the actual system libraries.*

### Environment

This repo contains a requirements.txt file with a list of all the packages and dependencies you will need. Before you install the virtual environment, make sure to install postgresql if you haven't done it before.

```bash
brew update
brew install postgresql
```

In order to install the environment you can use the following commands:

```
pyenv local 3.9.8
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```


### Notebooks

You can find the notebook used to perform the EDA as EDA_clean.ipynb. If you seek to know about analysis, which were later discarded (e.g.FFT), you may want to have a look at the EDA.ipynb. Furthermore you find the presenation for the client in form of the keynote presenation and as a pdf. 