Our top priority is doing reproducible science. This means establishing an efficient workflow that allows for collaboration in a convenient manner. The following set of guidelines and suggestions aim to this objective.

## Onboarding

There are a few things that each new member should do when he/she joins the research team. These are:

* Create a GitHub account.
* Check that your owncloud account is working.
* We use the slack for communication and wrike for project management. Make sure that you have been invited to both of them. 
* Download and begin to maintain a reference manager. We recommend [Zotero](https://www.zotero.org/), as the free software interfaces well with both Microsoft Word and Google Docs. 

## Data management

* We generally use a folder called "data" within each repository.
* We keep our raw data in the github repository related to the project, unless the data files are too large.
* We store our raw data with metadata describing what’s in the file and what the columns mean. We consider this data as read-only.
* If we clean the data, we often use a folder called something like "raw" to differentiate data in its original form from data that has been manipulated.
* If we are using data downloaded from another data source, we include the data source in a README.
* If our data are too large to store on GitHub, we store them in owncloud and include the link to README file for reproducibility.

## Analysis

* We do our data analysis in GitHub repositories to facilitate collaboration and sharing.
* We use scripts to process data, make models, do analyses, etc. and avoid spreedsheets, gis applications or other software.
* We follow some common scripting practices described [here](https://github.com/KVHEM/how_we_work/blob/master/CONTRIBUTING.md).
* `R` is used by the most team members and the `data.table`, `ggplot2` packages in specific. Of course other software/packages are welcome. 

## Results-Presentation

* We publish git repositories through [Zenodo](https://zenodo.org/) upon publication of a manuscript.
* Collaborative manuscripts are written either in [Overleaf](https://www.overleaf.com/) or [Google Drive](https://www.google.com/drive/).

## Guides and tutorials

* [R for data science](https://r4ds.had.co.nz/)
* [Rstudio with GitHub](https://www.rstudio.com/resources/webinars/rstudio-essentials-webinar-series-managing-part-2/)
* [R with git](https://happygitwithr.com/index.html)
* [Zotero](https://www.youtube.com/watch?v=q6-YOPS1xY4)
* [data.table vignette](https://cran.r-project.org/web/packages/data.table/vignettes/datatable-intro.html)

## Acknowledgements

Much of the inspiration for preserving an efficient, reproducible workflow came from [openscapes](https://www.openscapes.org/about/), while some of the material used here were copied from [Pinsky lab](https://github.com/pinskylab).
