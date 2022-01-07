# Agendas/Minutes

## 2022-01-21 | Intro to python
* 

## 2022-01-14 | 
* project updates
* should we reschedule?
* new members project discussion
    * Carolina: GEE+colab machine learning. Take over Luis's project? Will return on the 21st.
* 

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

