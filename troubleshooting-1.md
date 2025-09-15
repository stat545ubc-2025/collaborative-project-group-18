STAT 545A Troubleshooting Exercise for Milestone 1
================

There are **3 code chunks with errors** in this Rmd. Your objective is
to fix all of the errors in this worksheet. Make sure to indicate what
lines you changed and why (by commenting \# in the code).

For the purpose of grading, each erroneous code chunk is equally
weighted.

## Welcome to R and Rmd!

This document is written in **R Markdown**. We’ll use this document to
explore the `mtcars` dataset.

First, let’s store the current date as a variable. We can use the
function `Sys.Date` with no arguments to get the current date:

``` r
## ERROR 1 ##
today_ <- Sys.Date()

#fixed error to rename variable from _today_ to today_ in line 18
```

You may notice that, although an error might appear in these cells, this
Rmd file knits just fine. That’s because the `error = TRUE` *chunk
option* is included in each chunk, allowing the Rmd file to knit, even
when an error is encountered.

Now, let’s load the `tidyverse` (meta-) package:

``` r
## ERROR 2 ##
install.packages("tidyverse")
```

    ## Installing package into 'C:/Users/audre/AppData/Local/R/win-library/4.5'
    ## (as 'lib' is unspecified)

    ## Error in contrib.url(repos, "source"): trying to use CRAN without setting a mirror

``` r
library("tidyverse")
```

    ## ── Attaching core tidyverse packages ──────────────────────── tidyverse 2.0.0 ──
    ## ✔ dplyr     1.1.4     ✔ readr     2.1.5
    ## ✔ forcats   1.0.0     ✔ stringr   1.5.2
    ## ✔ ggplot2   4.0.0     ✔ tibble    3.3.0
    ## ✔ lubridate 1.9.4     ✔ tidyr     1.3.1
    ## ✔ purrr     1.1.0

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()
    ## ℹ Use the conflicted package (<http://conflicted.r-lib.org/>) to force all conflicts to become errors

``` r
#fixed error by installing package in line 30 and changing line 31 from libraries(tidyverse) to library("tidyverse")
```

By loading the tidyverse, a function called `glimpse` has been made
available. This function is useful for viewing a data set. Let’s take a
look at the `mtcars` dataset by applying the `glimpse` function to
`mtcars`!

``` r
## ERROR 3 ##
glimpse mtcars
```

    ## Error in parse(text = input): <text>:2:9: unexpected symbol
    ## 1: ## ERROR 3 ##
    ## 2: glimpse mtcars
    ##            ^

## Attribution

Thanks to Icíar Fernández Boyano for coming up with most of this
worksheet.
