jsmodule
================

[![Build Status](https://travis-ci.org/jinseob2kim/jsmodule.svg?branch=master)](https://travis-ci.org/jinseob2kim/jsmodule) [![AppVeyor build status](https://ci.appveyor.com/api/projects/status/github/jinseob2kim/jsmodule?branch=master&svg=true)](https://ci.appveyor.com/project/jinseob2kim/jsmodule) [![CRAN\_Status\_Badge](https://www.r-pkg.org/badges/version/jsmodule)](https://cran.r-project.org/package=jsmodule) [![CRAN\_Download\_Badge](https://cranlogs.r-pkg.org/badges/jsmodule)](https://CRAN.R-project.org/package=jsmodule) [![codecov](https://codecov.io/github/jinseob2kim/jsmodule/branch/master/graphs/badge.svg)](https://codecov.io/github/jinseob2kim/jsmodule) [![GitHub issues](https://img.shields.io/github/issues/jinseob2kim/jsmodule.svg)](https://github.com/jinseob2kim/jsmodule/issues) [![GitHub stars](https://img.shields.io/github/stars/jinseob2kim/jsmodule.svg)](https://github.com/jinseob2kim/jsmodule/stargazers) [![GitHub license](https://img.shields.io/github/license/jinseob2kim/jsmodule.svg)](https://github.com/jinseob2kim/jsmodule/blob/master/LICENSE)

RStudio Addins and Shiny Modules for Medical Research

Install
-------

``` r
install.packages("jsmodule")
library(jsmodule)

## From github: latest version
remotes::install_github('jinseob2kim/jsmodule')
```

RStudio Addins
--------------

### Basic statistics

Use `jsBasicGadget(data)` or Click **Basic statistics** Addin with **the dragged name of data**.

``` r
jsBasicGadget(mtcars)
```

![](vignettes/figures/addin.gif)

### Basic statistics with external data

Use `jsBasicExtAddin()` or Click **Basic statistics with external data** Addin **without any drag**

``` r
jsBasicExtAddin()
```

### Repeated measure analysis

Use `jsRepeatedGadget(data)` or Click **Repeated measure analysis** Addin with **the dragged name of data**.

``` r
jsRepeatedGadget(mtcars)
```

### Repeated measure analysis with external data

Use `jsRepeatedExtAddin()` or Click **Repeated measure analysis with external data** Addin **without any drag**

``` r
jsRepeatedExtAddin()
```

### Survey data analysis

Use `jsSurveyGadget(data)` or Click **Survey data analysis** Addin with **the dragged name of data**.

``` r
library(survey)
data(api)
jsSurveyGadget(apistrat)
```

### Survey data analysis with external data

Use `jsSurveyExtAddin()` or Click **Survey data analysis with external data** Addin **without any drag**

``` r
jsSurveyExtAddin()
```

### Propensity score analysis

Use `jsPropensityGadget(data)` or Click **Propensity score analysis** Addin with **the dragged name of data**.

``` r
jsPropensityGadget(mtcars)
```

![](vignettes/figures/ps.png)

### Propensity score analysis with external data

Use `jsPropensityExtAddin()` or Click **Propensity score analysis with external data** Addin **without any drag**

``` r
jsPropensityExtAddin()
```

Web applications
----------------

-   Basic statistics: <http://app.zarathu.com/basic>

-   Repeated measure analysis: <http://app.zarathu.com/repeated>

-   Survey data analysis: <http://app.zarathu.com/survey>

-   Propensity score analysis(experimental): <http://app.zarathu.com/ps>
