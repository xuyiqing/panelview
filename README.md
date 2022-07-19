
<!-- README.md is generated from README.Rmd. Please edit that file -->

# panelView

<!-- badges: start -->

[![Lifecycle:
stable](https://img.shields.io/badge/lifecycle-stable-green.svg)](https://www.tidyverse.org/lifecycle/#stablel)
[![License:
MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<!-- badges: end -->

**Authors:** Hongyu Mou (UCLA); Licheng Liu (MIT); [Yiqing
Xu](https://yiqingxu.org/) (Stanford)

**Date:** July 17, 2022

**Repos:** [Github](https://github.com/xuyiqing/panelView) (1.1.10)
[CRAN](https://cran.r-project.org/web/packages/panelView/index.html)
(1.1.9)

**Examples:** R code used in the tutorial can be downloaded from
[here](https://yiqingxu.org/packages/panelview/examples.R).

------------------------------------------------------------------------

## Description

**panelView** visualizes panel data. It has three main functionalities:

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

# note: "V" is capitalized
devtools::install_github('xuyiqing/panelView') 
```

You can also install the **panelView** package from CRAN:

``` r
install.packages('panelView') 
```

If you encounter an installation/execution error, please remove the old
package and reinstall **panelView**.

``` r
remove.packages('panelView') 
# or
remove.packages('panelview') # package name "panelview" no longer in use
```

## Example

For example, plot treatment status in a panel dataset:

``` r
library(panelView)
data(panelView)
panelview(turnout ~ policy_edr + policy_mail_in + policy_motor, 
          data = turnout, index = c("abb","year"), 
          xlab = "Year", ylab = "State")
```

Note that “V” in the package name is capitalized while “v” in the
function name is not—to be consistent with the Stata version. See
[tutorial](https://yiqingxu.org/packages/panelview/articles/tutorial.html)
for more details.

## Report bugs

Please report bugs to **yiqingxu \[at\] stanford.edu** with your sample
code and data file. Much appreciated!
