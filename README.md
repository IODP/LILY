# About

This repository is provided as a supplement to the LILY Database, downloadable at https://zenodo.org/record/8408296.

# Viewing Notebooks

Jupyter Notebooks will render in the browser. Click files with the ".ipynb" extension to view contents.

Alternatively, run notebooks in Jupyter Notebooks or Visual Studio Code with the Jupyter extension. Steps for creating a notebook kernel and installing the necessary packages are in the [Installation](#Installation) section

## AVS
LILY-AVS.ipynb only uses AVS_DataLITH.csv as input data. All output files are saved the "output" folder.

## RSC

LILY-RSC.ipynb references RSC_DataLITH.csv, it must be manually downloaded from Zenodo.

# Installation

The guide below walks through downloading the git repo from Github and creating a new virtual environment in Python containing the relevant Python packages listed in the requirements.txt file.

### Clone repo from Github
Run command from shell. Git commandline tools must be installed.

```shell
# verify git commandline tools are installed
git --version

# clone repo to local folder
git clone https://github.com/IODP/LILY.git
```


### Create new python virtual environment using Anaconda shell

Create a new virtual environment to ensure the repo artifacts are run against a compatible python version with the necessary packages installed. These instructions must be run within a conda shell. Alternatively, commands for creating new virtual environments directly in python may be found online.


```shell
# list virtual environments
conda info --envs

# create new virtual environment called "iodp" targeting python version 3.9
conda create -y --name iodp python=3.9

# activate newly created environment
conda activate iodp

# install packages listed in requirements.txt. Use full or relative path to requirements file if needed.
pip install --file requirements.txt

# deactivate environment to return to default base python environment
conda deactivate 

# Extra: step to remove environment. Run to delete environment and packages.
conda remove --name iodp --all
```




