# python-tech-workgroup
Welcome to the IMaRS python technical working group!

This repository is used to organize meetings & projects for anyone interested in learning how to leverage python coding in their research. 
We focus specifically on IMaRS research topics but all are welcome to join. 
If you would like to join the workgroup or get more information please email Tylar: mail@tylar.info
You may also jump right in and contribute to the projects listed below.

----------------------------------------------------------------------

To explore the demonstrational material in this repository click the badge below to open this repository using mybinder.org.
Once it has loaded you can open the `.ipynb` project files and explore.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/USF-IMARS/python-tech-workgroup/HEAD)

----------------------------------------------------------------------

## Projects
Workgroup memebers are currently working on the following projects:

project title                                                | members   | description
------------------------------------------------------------ | --------- | -----------------
[L2 processing](https://github.com/USF-IMARS/l2-processing)  | Dan       | processing MATLAB -> Python. streamline seascape products, working w/ Joaquin, grabbing extant from ERDDAP. doing the L2 processing, create means, do mapping.
[BB3 matchup](https://github.com/USF-IMARS/bb3_matchup)      | Sebastian | WS cruise align backscatter & depth data
[gee_notebooks](https://github.com/USF-IMARS/gee_notebooks)  | Luis      | analyses using GEE products, 3d wetlands data, & seagrass occurrences

----------------------------------------------------------------------

### steps for installing dependencies in your repos:
Use the various [binder configuration files](https://mybinder.readthedocs.io/en/latest/using/config_files.html) in the following order:
1. try to install your python dependency using `environment.yml` 
    * NOTE: similarly, you should use `DESCRIPTION` for `R` and `Project.toml` for Julia 
3. try to install your dependency using `apt.txt` to install ubuntu "`apt-get`" packages
4. run arbitrary bash commands using a `postBuild` file
5. create your own `Dockerfile` to replace all of the above

----------------------------------------------------------------------

### additional resources
Below is a list of related links that may be helpful.

* [intro to earth & enviro science in python](https://earth-env-data-science.github.io//intro.html) : gives good overview of basic tech like git, jupyter, unix, pandas, xarray, dask. Especially recommended is the "Geoscience package" section on mapping.
