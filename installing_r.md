# Installing R, RStudio and Packages

[![IMAGE ALT TEXT](http://img.youtube.com/vi/BJvWHs6ytEI/0.jpg)](http://www.youtube.com/watch?v=BJvWHs6ytEI "Video Title")

## New version of `R`

The video describes how to install `R` `3.5.0`. Version `3.5.1` is now out and you can install it instead.

## Packages

The video shows how to install the packages `{cowsay}` and `{ggplot2}`, but we need a lot more packages for the course. 

> By the way, when talking about packages we will use the convention to put their name in between curly brackets. That makes it easier to know what we are talking about when packages have common names, like package `{janitor}`.

You can run the code below in RStudio `Console` tab to install all the packages in one go:

```r
install.packages(c(
  "tidyverse",
  "rmarkdown",
  "janitor",
  "openxlsx",
  "datapasta",
  "dbplyr",
  "DBI",
  "odbc", 
  "RSQLite",
  "shiny",
  "devtools",
  "fs",
  "here",
  "ggmap",
  "leaflet"))
```

When the code is finished running, also run the line below. It needs to use the package `devtools` that we just installed: that's why we need to do it after the first big install.

```r
devtools::install_github("ropenscilabs/gramr")
```

##### Copy/Paste the code in the console and press enter

![](https://gist.githubusercontent.com/xvrdm/1bd7c5d665d40094f11aa22b51748e49/raw/15fd5e38989972ae9f86fc691d2170601ac21129/rstudio-install.gif)