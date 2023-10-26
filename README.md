
<!-- README.md is generated from README.Rmd. Please edit that file -->

# tutor

<!-- badges: start -->

[![CRAN
status](https://www.r-pkg.org/badges/version/tutor)](https://CRAN.R-project.org/package=tutor)
[![check-standard](https://github.com/ThinkR-open/tutor/actions/workflows/check-standard.yaml/badge.svg)](https://github.com/ThinkR-open/tutor/actions/workflows/check-standard.yaml)
[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
<!-- badges: end -->

The goal of tutor is support UNHCR staff self-learning

## Installation

``` r
# install.packages("devtools")
remotes::install_github("unhcRverse/tutor")
```

## Available tutorials

The list below includes tutorials from ThinkR -

UNHCR specific tutorial are prefaced `unhcr_`

``` r
## Run this to see all tutorials available
tutor::launch_learn() 

 ## Data Manipulation
 tutor::tibbles_en() 
 tutor::tibbles_fr() 
 tutor::join_datasets_en() 
 tutor::join_datasets_fr() 
 tutor::reshape_data_en() 
 tutor::reshape_data_fr()  
 tutor::separate_columns_en() 
 tutor::separate_columns_fr() 
 tutor::deriving_en() 
 tutor::deriving_fr() 
 tutor::isolating_en() 
 tutor::isolating_fr() 
 tutor::exploratory_data_analysis_en() 
 tutor::exploratory_data_analysis_fr()

## Creating Charts
 tutor::vis_basics_en()
 tutor::bar_charts_en() 
 tutor::bar_charts_fr() 
 tutor::boxplots_en() 
 tutor::boxplots_fr()  
 tutor::histograms_en() 
 tutor::histograms_fr() 
 tutor::line_graphs_en() 
 tutor::line_graphs_fr() 
 tutor::scatterplots_en() 
 tutor::scatterplots_fr() 
 
## Customise plots 
 tutor::customize_en() 
 tutor::customize_fr() 
 tutor::overplotting_en() 
 tutor::overplotting_fr() 
 
 ## Programming
 tutor::programming_basics_en() 
 tutor::programming_basics_fr()
```

## For Facilitator: Create your own tutorial

Please fork this repository, build your tutorials and submit them back
through Pull Request

This packages leverage the function from [Rstudio learnr
package](https://rstudio.github.io/learnr), such as the capacity for
your tutorial to include [Interactive
Questions](https://rstudio.github.io/learnr/reference/index.html#interactive-questions),
through quiz and other features…

    # new tutorial can be created with 
    library(tutor)
    source("R/create_learn_project.R")
    create_learn_project(
       name = "UNHCR_Tutorial_test2",
       path = "inst/tutorials",
       lang = "en" )
    ## you will then get a new Rmd files to edit in order to set up your tutorial
    ## once done, rebuild your package to test the tutorial
    # you can then launch your tutorial with 
    tutor::UNHCR_Tutorial_test2()
