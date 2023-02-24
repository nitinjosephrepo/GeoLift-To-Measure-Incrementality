# Measuring Incrementality With GeoLift


## Overview

GeoLift is an end-to-end solution to measure Lift at a Geo-level using the latest developments in Synthetic Control Methods. Through this tutorial it is possible to run Geolift R functions as power calculations, inference and plots in Python. 

Check out the files below for a more detailed description of the main functionalities of the package:

- GeoLiftPythonWalkthrough.ipynb: the completed GeoLift walkthrough in python including GeoLift single and multicell.

- demo.py: a simple GeoLift walkthrough in Python including only GeoLift single cell.


## Requirements 

GeoLift in Python version requires or works with:

- R version 4.0.0 or newer. Please check [R installaton](https://facebookincubator.github.io/GeoLift/docs/GettingStarted/InstallingR).

- Python version 3.7.0 or newer. Please check [Python installation](https://www.python.org/).


## Installation

The installation of GeoLift in Python version assumes that you will use pip3 as your Python package manager. If you do not use pip3, before running anything, edit the commands in setup.sh and change pip3 to your Python package manager to avoid package management issues.

### Option 1 - Work environment

Step 1: Download GeoLiftPython folder hosted on GeoLift's Github.

Step 2 (On Terminal): Located in the GeoLiftPython folder, run the commands below in your environment: 

```
pip3 install -r requirements.txt
python3 r_lang_requirements.py
```

Step 2 (On Jupyter): Located in the GeoLiftPython folder, run the commands below in your environment: 

```
!pip3 install -r requirements.txt
%run r_lang_requirements.py
```

These commands will:
1.1 install the `pandas`, `rpy2`, `ipython`, `jupyter` packages under `requirement.txt`.
1.2 install `augsynth` and `Geolift` R packages in `r_lang_requirements.txt`.

NOTE: 
If you don't want to install Jupyter, you can remove jupyter from requirements.txt

### Option 2 - Virtual environment (MacOS only)

Step 1: Download GeoLiftPython folder hosted on GeoLift's Github.

Step 2: In your terminal, go to the GeoLiftPython folder and run the following:
```
bash setup.sh
```
This command will:
1.1 install `virtualenv` python package and activate a virutal environment. 
1.2 install the `pandas`, `rpy2`, `ipython`, `jupyter` packages under `requirement.txt`.
1.3 install `augsynth` and `Geolift` R packages in `r_lang_requirements.txt`.
1.4 open Jupyter Notebook.

Step 3: Open the `GeoLiftPython.ipynb` directly from your Jupyter Notebook interface.

NOTE: 
If you have closed your notebook, there is no need to reinstall everything.  All you need to do is reactivate your virtualenv with:

```
source path/to/GeoLiftPython/venv_geolift_python/bin/activate
jupyter notebook
```
If your GeoLift files are in a different folder than the one activated, you need to go to the folder where your GeoLift files are located before running `jupyter notebook`.


Happy GeoLifting!



