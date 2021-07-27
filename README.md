
<!-- README.md is generated from README.Rmd. Please edit that file -->

# scenarioSelector <a href='https://github.com/2DegreesInvesting/r2dii.usethis'><img src='https://imgur.com/A5ASZPE.png' align='right' height='43' /></a>

<!-- badges: start -->

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/scenarioSelector)](https://CRAN.R-project.org/package=scenarioSelector)
[![R-CMD-check](https://github.com/2DegreesInvesting/scenarioSelector/workflows/R-CMD-check/badge.svg)](https://github.com/2DegreesInvesting/scenarioSelector/actions)
[![Codecov test
coverage](https://codecov.io/gh/2DegreesInvesting/scenarioSelector/branch/master/graph/badge.svg)](https://codecov.io/gh/2DegreesInvesting/scenarioSelector?branch=master)
<!-- badges: end -->

The goal of the scenarioSelector
[app](https://twodii.shinyapps.io/scenarioSelector/) is to help you find
and visualize a scenario.

## Installation

Install the development version of scenarioSelector from GitHub with:

``` r
# install.packages("devtools")
devtools::install_github("2DegreesInvesting/scenarioSelector")
```

## Example

``` r
if (interactive()) {
  scenarioSelector::run_app()
}
```

## Discussion

For a discussion including related work see the channel
[`# scenario-selector-tool`](https://2investinginitiative.slack.com/archives/C025YFS5UTA)
on 2DII’s Slack or [ADO
\#552](https://dev.azure.com/2DegreesInvesting/2DegreesInvesting/_workitems/edit/552).

## Learning shiny

This app is small but implements some big ideas I learned from
[Mastering Shiny, by Hadley Wickham](https://mastering-shiny.org/):

-   [Packages](https://mastering-shiny.org/scaling-packaging.html)
    ([code](https://github.com/2DegreesInvesting/scenarioSelector/blob/master/DESCRIPTION)).

-   [Shiny modules](https://mastering-shiny.org/scaling-modules.html)
    ([code](https://github.com/2DegreesInvesting/scenarioSelector/blob/master/R/scenario.R)).

-   [Testing
    reactivity](https://mastering-shiny.org/scaling-testing.html#testing-reactivity)
    ([code](https://github.com/2DegreesInvesting/scenarioSelector/blob/master/tests/testthat/test-scenario.R)).

-   [UI as
    data](https://mastering-shiny.org/scaling-functions.html#ui-as-data)
    ([code](https://github.com/2DegreesInvesting/scenarioSelector/blob/master/R/select_column.R)).

-   [Server
    functions](https://mastering-shiny.org/scaling-functions.html#server-functions)
    ([code](https://github.com/2DegreesInvesting/scenarioSelector/blob/master/R/plot_scenarios.R)).

-   [Hierarchical select
    boxes](https://mastering-shiny.org/action-dynamic.html?q=hiera#hierarchical-select)
    ([code](https://github.com/2DegreesInvesting/scenarioSelector/blob/master/R/scenario.R)).
