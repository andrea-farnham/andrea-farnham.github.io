# GLOMOH - GLObal MObility and Health

Welcome to our site 

- Website URL <https://andrea.farnham.pages.uzh.ch/climah/>



## About this site
Information for mantainers: 

- **.gitlab-ci.yml**: this file defines the Continous Integration pipeline. It has the script that pulls the docker container, installs additional packages and runs the main action `quarto render` to update the website. Any change in this repository triggers this pipeline (it takes 2-3 minutes to run). The result of the pipeline (the website and all HTML files that compose it) will not be visible in the repository, but as an `artifact`. Thus, the HTMLs with the website can be found in the Gitlab menu: `Build>Artifacts`

- **_quarto.yml**: this is the Quarto project file with the page layout and some settings. Some of the settings can be defined as well in the YAML section (the header) of the individual .qmd files. 

- **assets/**: this folder contains misc images and logos used in the site (landing page, navigation bar, footer, etc)

- **index.qmd**: the file at the root folder defines the content for the landing site. The index.qmd inside each of the other folders (e.g., about/index.qmd) define the content of the other pages. There may be multiple .qmd files inside a folder, but only one index.qmd. The index.qmd can contain a 'listing' field in the header: this is used by QUARTO to list the different .qmd files in a page (e.g., as tiles or as a table)

- **other folders/**: each page has its own folder. It must contain an index.qmd and it may contain an folder with images or other assets used in the page. 











