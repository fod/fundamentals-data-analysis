# Fundamentals of Data Analysis Assessment Repository

This repository contains two [Jupyter](https://jupyter.org/) notebooks and ancillary files demonstrating some aspects of data analysis using the Python programming language and various associated technologies in fulfillment of requirements for the *Fundamentals of Data Analysis* module of the HDipSc in Computing in Data Analytics at the Galway-Mayo Institute of Technology (GMIT). One notebook, [cao.ipynb](cao.ipynb) focuses on the acquisition, parsing, and cleaning of data in various file formats from online sources without a formal API, while the other, [pyplot.ipynb](pyplot.ipynb), focuses on data visualisation using the [Matplotlib](https://matplotlib.org/) Python plotting library.

## Repository Contents

The repository contains two Jupyter notebooks which are independent of one another;
- [cao.ipynb](cao.ipynb)
- [pyplot.ipynb](pyplot.ipynb)

The rest of the contents of the repository all support those files in some way. They are:
- README.md; this file
- [requirements.txt](requirements.txt); a list of Python packages required to run the notebooks
- .gitignore; a git support file which may be safely ignored
- [images/](images/); a directory containing some images which appear in the [CAO notebook](cao.ipynb)
- [data/](data/); a directory containing:
    - [ed_centroids.csv](data/ed_centroids.csv); a csv file contain geographic location information used in a plot in the [pyplot notebook](pyplot.ipynb)
    - [cao/](cao/); a directory containing files consumed or produced by the [CAO notebook](cao.ipynb):
    - a number of pdf, xslx, and html files containing data downloaded from the [CAO website](http://www.cao.ie/index.php?page=points&bb=mediastats) which is used by the [CAO notebook](cao.ipynb). These files follow the naming pattern 'cao_', + YYYY + '_lvl' + '8', '76', or '876'. YYYY is the year the data in the file refers to and the number after 'lvl' is the level of the courses listed in the file.
    - [cao/csv/](data/cao/csv/); a directory containing a number of csv files of parsed and cleaned CAO points data output by the [CAO notebook](cao.ipynb). These follow the namimg pattern 'cao_' + YYYY + '.csv', where YYYY is the year of the data held in the csv file. The file [cao_2001-2021.csv](data/cao/csv/cao_2001-2021.csv). Contains all of the data contained in the individual year files. This (or, indeed any of the other 'cao_' csv files), can be imported into the [CAO notebook](cao.ipynb) for analysis without having to wait for data regeneration from source. Any of these files can, of course, also be used independently for other analyses.
    - [cao/backup/](/data/cao/backup/); a directory containing an identical set of files as those found in the source files directory ([data/cao/](data/cao/)) but with a timestamp appended to each filename. This is a set of backup source files automatically generated by the [CAO notebook](cao.ipynb). Whenever the notebook is run it will check for changes to the source data, update it and back it up if found. Note that this system fails if the CAO change filename, format, or url for a resourse. As such, its purpose is to back up old source data which has been inadvertently updated to aid in bug and error management and mitigation. 

## Requirements

Nothing extra is required to view the contents of repository on [github](https://github.com/fod/fundamentals-data-analysis) or [nbviewer](https://nbviewer.org/) or [binder](https://mybinder.org/). However see [below](#how-to-run) for discussion of the limitations of these formats.

To run these notebooks locally [Python v3.9+](https://www.python.org/) with [Pip](https://pypi.org/project/pip/) or some other package manager is the minimum requirement. In order to clone this repository - the easiest way to acquire the code - [git v.2+](https://git-scm.com/) is required. The [Java Runtime Environment (JRE) 7+](https://www.java.com/en/download/manual.jsp) or [OpenJDK 7+](https://openjdk.java.net/) is required for some pdf parsing functionality in the [CAO notebook](cao.ipynb).

Assuming Python is installed then the Python packages listed in [requirements.txt](requirements.txt) are required. These can usually be installed in one go using the [requirements.txt](requirements.txt) file with pip or, presumably, any other Python package manager. See [below](#how-to-run) for details.

## How to run

There are three ways to consume the notebooks in this repository:
1. View here on github by simply clicking on [cao.ipynb](cao.ipynb) or [pyplot.ipynb](pyplot.ipynb), or on [nbviewer](https://nbviewer.org/) by clicking on the appropriate button:

    - For the CAO notebook:&ensp;&ensp;&ensp;[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/fod/fundamentals-data-analysis/blob/main/cao.ipynb)

    - For the pyplot notebook:&ensp;[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://github.com/fod/fundamentals-data-analysis/blob/main/pyplot.ipynb)


## CAO notebook

## pyplot notebook
