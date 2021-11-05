# python-tech-workgroup
2021 Fall IMaRS python technical working group

Use the badge below to open this repository using mybinder.org & open `.ipynb` project files.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/USF-IMARS/python-tech-workgroup/HEAD)

## projects spawned from here:
* [L2 processing](https://github.com/USF-IMARS/l2-processing) : Dan       : processing MATLAB -> Python
    * streamline seascape products, working w/ Joaquin, grabbing extant from ERDDAP
    * doing the L2 processing, create means, do mapping
* [BB3 matchup](https://github.com/USF-IMARS/bb3_matchup) : Sebastian : WS cruise align backscatter & depth data
* [gee_notebooks](https://github.com/USF-IMARS/gee_notebooks/tree/main) : Luis : analyses using GEE products, 3d wetlands data, & seagrass occurrences


--------------------------------------------

### steps for installing dependencies in your repos:
Use the various [binder configuration files](https://mybinder.readthedocs.io/en/latest/using/config_files.html) in the following order:
1. try to install your python dependency using `environment.yml` 
    * NOTE: similarly, you should use `DESCRIPTION` for `R` and `Project.toml` for Julia 
3. try to install your dependency using `apt.txt` to install ubuntu "`apt-get`" packages
4. run arbitrary bash commands using a `postBuild` file
5. create your own `Dockerfile` to replace all of the above

--------------------------------------------

### additional resources
Below is a list of related links that may be helpful.

* [intro to earth & enviro science in python](https://earth-env-data-science.github.io//intro.html) : gives good overview of basic tech like git, jupyter, unix, pandas, xarray, dask. Especially recommended is the "Geoscience package" section on mapping.
