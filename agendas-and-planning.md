## week 01 - 2021-09-17 - setup basics

### Learning Objectives Completed
* get set up with github
* overview of github issues, milestones
* overview of jupyter, binder, mybinder.org
* how to create `.ipynb` in github and load using mybinder.org
* the PEP8 python style guide

### Agenda:
* [X] review homework :book: issues/questions
* [X] test out the python environment
* [X] discuss possible projects
* [X] discuss possible invitees
* [X] establish a lead for each project

### TODO items:
* [X] create github issues "labels" for each project

## week 02 - 2021-09-24 - projects setup
### learning objectives completed:
* installing dependencies with `requirments.txt` & `environment.yml`
* basics of connecting data to mybinder.org containers
* quick demo of for loops, lists, and map().
* first glimpses of `parse`, `pandas`, `datetime`, `os` packages


## week 03 - 2021-10-01 - getting into a dev workflow

### Agenda:
* [ ] project updates
* [ ] :book: project lead creates a github issue (or multiple) documenting first steps for their project 

### project updates:
#### GEE
* new notebook added `L2_processing_GEE_in_colab.ipynb` for working w/ google colab
    * need to install anaconda for py6s
* other notebook needs minor porting from py2 to py3
* permissions issues when trying to use GEE (see #15)

#### MODIS processing
* files uploaded to github `/data/MODA_OC_py_data/`
* need to do filename parsing to get metadata from filename

#### Cruise data
* nothing new yet

### learning objectives completed:
* using lists, dicts, duck-typing, `str`
* datetime.strptime
* parse package to parse filenames

## week 04 - 2021-10-08 - ...
* ?

## week 05 - 2021-10-15 - 
* spatio-temporal interpolations - see #18

-----------------------------------------------------------------------------------

### Additional Topics to Cover:
* [ ] interpolation (spatial maps & time series)
* [ ] generating means, mosaics, climatologies
* [ ] file i/o for several file types
* [ ] fetching river or buoy data 
* [ ] ***downloading sat data***
* [ ] working with 3d matricies (numpy)
* [ ] plotting & visualizations (matplotlib)
* [x] filename/string parsing
* [x] packaging/dependecy management pip, pyenv, conda (esp. GDAL installation/setup)
* [x] basic best practices
* [ ] subprocess.run
* [ ] how (and why) to put functions into a .py file and import it to the ipynb
    * [ ] better VCS on .py files (commit diffs make sense instead of big json file replacement)
    * [ ] you don't need to use a jupyter notebook editor, any text editor works. 
    * [ ] you can build tests for your functions (test-driven development is a wonderful practice)

