# Data Science Lab Computer Vision course with Python
## 3. napari

This course is an introduction to the Python n-dimensional image visualizer napari. It is part of the [Data Science Lab](https://www.dsl.unibe.ch/) course on Computer Vision with Python. The goal of the course is to familiarize participants with napari a powerful image visualization software originally developed by the bioimaging community but usable with any type of images from other fields as well. The course is composed of three parts:
- main functionalities of napari and its layer system
- possibilities offered by napari extensions called plugins
- how to develop a plugin

In each part, explanations are provided in notebooks that one can just read or execute and modify. Exercises matching the content are suggested at the end of each notebook.

## Getting the material

To use all notebooks locally, you can simply clone (if you know git) or download the repository by using the green "Code" button at the top right of the repository. Place the folder in easily reachable location on your computer.

You can download all necessary data from [this link](). Place the main data folder then in the main folder of the downloaded repository for paths to be correct.

## Setting up an environment

A series of packages is necessary to run the content of this notebook. We highly recommend to install packages within an environment such as provided by conda. There are multiple ways to install conda and if you don't yet have a version installed we strongly recommend to use mambaforge which will install the fast environment solver mamba. You can find installers at [this link](https://github.com/conda-forge/miniforge#mambaforge). 

Note that you can use mamba also from an older conda installation. For this follow these steps (described [here](https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community):
1. Update conda:
    ```conda update -n base conda```
2. Install mamba:
    ```conda install -n base conda-libmamba-solver```
3. Use mamba as a solver:
    ```conda config --set solver libmamba```

Once you have conda/mamba installed, open a terminal where you have access to conda (i.e. the beginning of the line on your terminal window should indicate ```(base)```). On MacOS or Linux, your regular terminal should work. On Windows, depending how you installed conda, you might only have access to it from a terminal called "XXX Prompt" where XXX stands for Anaconda, Miniforge etc.

Then in that terminal move to the folder of the repository you downloaded previously (use ```cd path_to_your_folder```). In the main folder you will find an [environment.yml](environment.yml) file that contains infos about all packages to install. You can simply create the necessary environment using:

    mamba env create -f environment.yml

if you have mamba installed or

    conda env create -f environment.yml

This creates an environment called ```dslnapari``` that you then need to activate (here mamba or conda doesn't matter):

    conda activate dslpytorch

Finally you can start Jupyterlab using:

    jupyter lab

This should automatically open a Jupyterlab session in your favorite browser. If not, copy the address appearing in the terminal starting with ```http://localhost:8888...``` in your browser.

## Google Colab

Note that unlike the other parts of the course, you cannot run the notebooks on Colab as napari is a desktop application that cannot run remotely.

## Authors

Guillaume Witz, Data Science Lab, University of Bern