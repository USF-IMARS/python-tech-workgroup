# Agendas/Minutes

## 2022-0?-?? | Ben's extractR
* TODO: bother @bbest

## 2022-0?-?? | mapping & interpolations???
Focus on BB3 project interpolations?

## 2022-02-11 | python modules & directory structure???
Overview of L2 notebooks retooled to become a module.
* working w/ git submodules
* directory structure
* module setup
* (unit) testing w/ pytest

## 2022-02-04 | GEE + Google Collab
[Luis](https://github.com/luislizcano) will lead an overview of using google collab (a jupyterhub hosting alternative to mybinder.org) and how to use google earth engine within collab.
* overview of collab
* overview of finding, importing ImageCollection data in GEE code editor
* basic ImageCollection filtering
* how to display multiband ImageCollection
* how to do all the above in G Collab
* how to do mean, extract a timeseries, and plot it
* walkthrough example of creating SDM from GBIF data using SST, elevation, & precip.

## 2022-01-28 | mybinder.org Project Setup
* project updates:
    * [SOCCOM_eddy repo set up](https://github.com/Williams-OBGC-Lab/SOCCOM_eddy)
    * GEE next steps need to be done in Colab - demo next week! 
    * coral assessment - looking at more data & considering using GEE
        * want to create comprehensive map of coral data in the FL keys
        * starting from David Palandro(sp?)'s old data

## 2022-01-21 | Intro to python
* loading a data file
* Project updates:
    * Nicola : working on argo float data function
    * Chelsea : going to load in CREMP location + % cover data for plotting
    * Dan : awaiting module-ization 
    * Juan : awaiting data details
    * Claudia : water quality, SST, & CHL basics & plotting
    * Carolina : seagrass fish community video data processing (ML?). Extract & analyze OBIS data.
    * Mostafa : basics of python & python setup

## 2022-01-14 | Intro to the group
* project updates
    * None
* points of order
    * introductions
        * ensure everyone is:
            * on the teams event
            * in usf-imars org as member or collab 
    * should we reschedule? no
* intro to this workgroup 
    * if you don't have a github account, make one now.
    * Look at the [README](https://github.com/USF-IMARS/python-tech-workgroup#readme)
    * Open the project repo using "launch" mybinder.org button
    * Using github "issues" [here](https://github.com/USF-IMARS/python-tech-workgroup/issues)
* new members project discussions
    * GEE+colab machine learning. Take over Luis's project? Will return on the 21st.
    * Interpolation w/ API-pulled Argo/Saildrone data
    * FL Keys coral health over time
* homework: 
    1. create an issue
    2. tag it "discussion"
    3. propose a project idea
    4. review & comment on other people's discussion "issues"

## 2022-01-07
* project updates
    * L2 proc: 
         * GPT is too hard to install. OCSSW run bothered by [issue 1](https://github.com/USF-IMARS/l2-processing/issues/1).
         * Going to move this project out of jupyter notebooks. Dan choosing an IDE.
         * requested topics : functions, python files, CLI code, saving variables into pickle file.
    * GEE: 
         * requested topics : co-lab demo/intro, functions, python files
    * BB3: 
        * requested topics: data viz. "user stories"/goals for imagery:
            * time series analysis
            * depth profile plot
            * map w/ a cruise track
* possible additional members?
    * Nancy Williams's students
    * Niel Hammerschalg's Students
* prep for starting semester:
    * wanting to include new members; they will need projects
    * will focus meeting on generic topics better for new members
    * will push project-specific topics to github issues
        * please try to use github issues to document requests. this will help me plan the meetings.

-----------------------------------------------------------------------------------

# possible topics 2022 Spring
* plotting & viz basics
    * [sat data](https://gist.github.com/7yl4r/481912f04f0d7f9a848a4914ada4ed1b)

-----------------------------------------------------------------------------------

# Topic ideas:
* [ ] **python packaging directory structure**
* [ ] generating means, mosaics, climatologies
* [ ] fetching river or buoy data 
* [ ] ***downloading sat data***
* [ ] working with 3d matricies (numpy)
* [ ] subprocess.run
* [ ] data processing pipeline theory
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

