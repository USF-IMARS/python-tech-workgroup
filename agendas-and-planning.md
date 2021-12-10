# Topic ideas:
* [ ] **python packaging directory structure**
* [ ] interpolation 
* [ ] generating means, mosaics, climatologies
* [x] file i/o for several file types (`csv`, `nc`, `pickle`
* [ ] fetching river or buoy data 
* [ ] ***downloading sat data***
* [ ] working with 3d matricies (numpy)
* [ ] plotting & visualizations (matplotlib, plotly, seaborn, etc)
* [x] filename/string parsing
* [x] packaging/dependecy management pip, pyenv, conda (esp. GDAL installation/setup)
* [x] basic best practices
* [ ] subprocess.run
* [ ] some data processing pipeline theory
    * ETL (extract, transform, load) : process (transform) one data object (file) into another
    * data provenance : the history of everything that happens between data creation & final result
* [ ] spatio-temporal interpolations - see #18
    * on BB3 data?
    * on sea level rise prediction data for 3D wetlands? 
    * spatial maps & time series
* [ ] histograms
    * to see outliers & (assumed bi-modality) in BB3 data
    * 3d wetlands histograms of spatial data classes/values? (based on Luis's existing works)
* [ ] statistical outlier detection & removal
* [ ] PCA visualization / dimensionality reduction / unsupervised clustering
    * [ ] RDA? 
    * [ ] [biodiversityR](https://github.com/cran/BiodiversityR) / vegan package
* [ ] interactive components (silders, selectors, etc) in jupyter notebooks
* [ ] CLI building using argparse

* [ ] creating functions & "modules"
    * why?
        * don't need to use a jupyter notebook editor, any text editor works. 
        * can build tests for your functions (test-driven development is a wonderful practice)
        * **better VCS on .py files** (commit diffs make sense instead of big json file replacement)
        * shorten your notebook & don't repeat yourself (DRY)
        * **can use common functions between multiple notebooks/files (& projects by creating a package)**
    * how to put functions into a .py file and import it to the ipynb
        * walkthrough [obis_notebooks example](https://github.com/USF-IMARS/obis_notebooks/blob/master/dwc_download_and_analyze.ipynb)
            1. create & test using a function in the notebook
            2. move fn def to a `.py` file
            3. `import my_function from my_module`
* [ ] create an "atomic" data pipeline with one "main" notebook which calls functions, passing filenames as in/out

-----------------------------------------------------------------------------------

# possible topics 2022 Spring
* Luis co-lab demo
* review functions, modules, importing, opening files (csv, pickle)
* plotting & viz 

-----------------------------------------------------------------------------------

# weekly agendas/plans

## week 11 | 2021-12-10 | basic gridded data viz
* project updates
    * GPT installation?
    * l2 processing w/o GPT?
    * Co-Lab questions?
    * BB3 status update
 * basic data viz of MODIS/VIIRS (+ GEE?) imagery
 * TODO: identify data viz "user stories"/goals for imagery

## week 10 | 2021-12-03 | planning
For next semester: 
* project updates briefly at start then daily topic.
* walkthroughs using the notebooks

## week 09 | 2021-11-12 | functions, modules, & pipelines?
### project updates
* L2 SEADAS install is working?
* GEE pub topic ready?
* BB3 next steps?

### demonstrations
* load pickle files from URLs (see updated `04_reading_pickle_files.ipynb`)

## week 08 - 2021-11-05 - cleanups, functions, pickles
* L2 processing needs GPT installed via apt.txt and environment.yml
* GEE needs targeted research question(s) or publication goal to drive further development 

* we can create shared data by publishing "atomic" `.csv`, `.nc`, or `.pickle` files
    * atomic transforms : do one data transformation at a time, save files between each transform
* using the `pickle` package (& why)
    * pickle any object. see notebooks/instructional/02...
    * unpickle the file later. see notebooks/instructional/04...
    * files get big fast. TODO: try using bz2 compression [ref](https://betterprogramming.pub/load-fast-load-big-with-compressed-pickles-5f311584507e)

## week 07 - 2021-10-29 - new repos
* everybody create your own (binder-powered) repo!
* GEE examples for using maxent looks very promising [eg](https://code.earthengine.google.com/b1a0cc8c8ff49eadae115caadbbab3b8)

## week 06 - 2021-10-22 - playing w/ time series decomposition
## week 05 - 2021-10-15 - loading data into pandas
## week 04 - 2021-10-08 - debugging proj specifics
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

## week 02 - 2021-09-24 - projects setup
### learning objectives completed:
* installing dependencies with `requirments.txt` & `environment.yml`
* basics of connecting data to mybinder.org containers
* quick demo of for loops, lists, and map().
* first glimpses of `parse`, `pandas`, `datetime`, `os` packages


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
