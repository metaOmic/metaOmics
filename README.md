# metaOmics
A graphical user interface to facilitate the application of meta analysis on -Omics study

## Required package
preproc, metaClust, DT, shiny, shinyBS

## How to start the app
if the directory of the app is `metaOmics`,
* in command line:
```
R -e "shiny::runApp('metaOmics', port=9987, launch.browser=T)"
```
* in R
```R
shiny::runApp('metaOmics', port=9987, launch.browser=T)
```

## How to start the documentation

* Install rmarkdown for R
```
instal.packages("rmarkdown")
```
* Inside `doc` directory, start R console, and:
```R
rmarkdown::run(shiny_args=list(port=9988, launch.browser=T))
```
or in command line
```
R -e "rmarkdown::run(shiny_args=list(port=9988, launch.browser=T))"
```
* If you run into an issue with something like `pandoc version 1.12.3 or higher is required and was not found.`, just install pandoc manually. For example, on Mac, it would be `brew install pandoc`. If you have Rstudio, you need to get r studio's pandoc environment. Go to rstudio console and  find the system environment variable for `RSTUDIO_PANDOC`
```R
Sys.getenv("RSTUDIO_PANDOC")
```
