# Archived

This is an archived repository. For active repositories related to CyAN/GLRI, see:
(CyAN-Web)[https://github.com/USGS-WiM/CyAN-Web]
(CyAN_DB)[https://github.com/USGS-WiM/CyAN_DB]

# CyAN

This package provides a set of tools for working with the database developed for the [Cyanobacterial Assessment Network](https://www.epa.gov/water-research/cyanobacteria-assessment-network-cyan). CyAN is a cooperation between NASA, NOAA, EPA and USGS with the goal of detecting freshwater algal blooms early using satellite data.

## Installation

To use the CyAN package, you should be using R 3.5+. You can install the package from GitHub using the `remotes` package. To build the vignette (long-form documentation) included with the package, you'll need the `knitr` and `markdown` libraries installed.

To install all 3 packages:

```r
install.packages(c("remotes", "knitr", "rmarkdown"))
```

Then to install the package with vignettes:

```r
remotes::install_github("USGS-R/CyAN", build_vignettes = TRUE)
```

Or to install the package without the vignette:

```r
remotes::install_github("USGS-R/CyAN")
```

## Using the package

First load the package:

```
library(CyAN)
```

For an introduction to the package, and to see an example workflow, view the package vignette:

```r
vignette("CyAN")
```

This package also includes an interactive app that can be used for exploring available data and downloading subsets of the data in csv files. The application will launch in a browser window. To run the app:

```r
run_CyAN()
```

## Disclaimer

This software is in the public domain because it contains materials that originally came from the U.S. Geological Survey, an agency of the United States Department of Interior. For more information, see the official USGS copyright policy

Although this software program has been used by the U.S. Geological Survey (USGS), no warranty, expressed or implied, is made by the USGS or the U.S. Government as to the accuracy and functioning of the program and related program material nor shall the fact of distribution constitute any such warranty, and no responsibility is assumed by the USGS in connection therewith.

This software is provided "AS IS."
