
<!-- README.md is generated from README.Rmd. Please edit that file -->

# panelview

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![License:
MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<!-- badges: end -->

**Authors:** Hongyu Mou (PKU); Licheng Liu (MIT); [Yiqing
Xu](https://yiqingxu.org/) (Stanford)

**Date:** Feb 1, 2022

**Repos:** [Github](https://github.com/xuyiqing/panelview) (1.1.8)
[CRAN](https://cran.r-project.org/web/packages/panelView/index.html)
(1.1.5)

**Examples:** R code used in the tutorial can be downloaded from
[here](https://yiqingxu.org/packages/panelview/panelview_examples.R).

------------------------------------------------------------------------

## Description

**panelview** visualizes panel data. It has three main functionalities:

1.  it plots treatment status and missing values in a panel dataset;
2.  it plots an outcome variable (or any variable) in a time-series
    fashion;
3.  it visualizes bivariate relationships of two variables by unit or in
    aggregate.

## Installation

You can install the up-to-date development version from GitHub:

``` r
# if not already installed
install.packages('devtools', repos = 'http://cran.us.r-project.org') 

# currently, v.1.1.8 ("v" is not capitalized)
devtools::install_github('xuyiqing/panelview') 
```

You can also install the **panelview** package from CRAN:

``` r
# currently, v.1.1.5 ("V" is capitalized; we'll update it soon)
install.packages('panelView') 
```

## Example

For example, plot treatment status in a panel dataset:

``` r
library(panelview)
panelview(turnout ~ policy_edr + policy_mail_in + policy_motor, 
          data = turnout, index = c("abb","year"), 
          xlab = "Year", ylab = "State")
```

See
[tutorial](https://yiqingxu.org/packages/panelview/articles/tutorial.html)
for more details.

## Report bugs

Please report bugs to **yiqingxu \[at\] stanford.edu** with your sample
code and data file. Much appreciated!
