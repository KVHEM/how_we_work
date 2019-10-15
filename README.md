Reproducible science is our top priority. Therefore, it is imperative to establish an efficient workflow that allows for collaboration in a convenient manner. To achieve those above, please stick to the guidelines and suggestions below as much as possible.

## Onboarding

Every new member that joins the research team should:

* Create a GitHub account.
* Verify that [owncloud](https://owncloud.cesnet.cz/)  account is active and working.
* Slack is used for communication and Wrike for project management. Make sure to have been invited to both of them. 
* Download and start to maintain a reference manager. We recommend [Zotero](https://www.zotero.org/), as the freeware is compatible with both Microsoft Word and Google Docs. 
* Read the standard scripting practices described [here](https://github.com/KVHEM/how_we_work/blob/master/CONTRIBUTING.md).

## Data management

* In general, we use a folder called "data" within each repository.
* If data comes from another data source, we include the data source in a README.
* Raw data is available in the corresponding GitHub repository unless file-size is too large (> 100MB).
* When data file-size is too large, we store it in owncloud and include the link to the README file for reproducibility.
* When storing raw data, always include metadata describing what is in the file and what the columns mean. Remember, we consider this data as read-only.
* If we clean the data, we use a folder called "raw" or similar to differentiate original data from manipulated data easily.
* Some useful suggestions and ideas can be found in the [Cambridge Data Management Website](https://www.data.cam.ac.uk/data-management-guide/organising-your-data).

## Analysis

* We do our data analysis in GitHub repositories to facilitate collaboration and sharing.
* We use scripts to process data, make models, do analyses, and many others. In addition, we avoid spreadsheets, gis applications, or other software.
* `R` is used by most team members and the `data.table`, `ggplot2` packages in specific. Of course, other software/packages are welcome. 
* We try to comment a lot in our code.

## Results-Presentation

* We aim to fully reproducible papers, like this [example](https://github.com/CenterForOpenScience/rpp/blob/master/README.md). 
* We publish git repositories through [Zenodo](https://zenodo.org/) upon publication of a manuscript.
* Collaborative manuscripts are written either in [Overleaf](https://www.overleaf.com/) or [Google Drive](https://www.google.com/drive/).

## Guides and tutorials

* [R for data science](https://r4ds.had.co.nz/)
* [R/R studio for pure beginners](https://swcarpentry.github.io/r-novice-gapminder/01-rstudio-intro/index.html)
* [Rstudio with GitHub](https://www.rstudio.com/resources/webinars/rstudio-essentials-webinar-series-managing-part-2/)
* [R with git](https://happygitwithr.com/index.html)
* [Zotero](https://www.youtube.com/watch?v=q6-YOPS1xY4)
* [data.table vignette](https://cran.r-project.org/web/packages/data.table/vignettes/datatable-intro.html)
* [writing good software](https://swcarpentry.github.io/r-novice-gapminder/16-wrap-up/index.html)

## Acknowledgements

Much of the inspiration for preserving an efficient, reproducible workflow came from [openscapes](https://www.openscapes.org/about/), while some of the material used here was adapted from [Pinsky lab](https://github.com/pinskylab).
