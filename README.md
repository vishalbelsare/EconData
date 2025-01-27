EconData
================
Created by Bradley Setzler, Pennsylvania State University

This is a directory for managing publicly-available economics data. It
contains two components:

-   [EconData](https://github.com/setzler/EconData/tree/master/EconData):
    R package to automatically download and prepare various
    publicly-available economic data sets from source.
-   [DataRepo](https://github.com/setzler/EconData/tree/master/DataRepo)
    A repository of prepared data sets that were created by the EconData
    package.

To use the R package, run the following:

``` r
devtools::install_github("setzler/EconData/EconData")
```

``` r
library(EconData)
```

Data sets currently available include:

-   [State corporate tax
    rates](https://github.com/setzler/EconData/tree/master/DataRepo/StateCorpTax/),
    covering all states during 2000-2020.
-   [Census
    CBP](https://github.com/setzler/EconData/tree/master/DataRepo/CensusCBP/)
    employment, earnings, and establishments at various levels of
    aggregation, 2001-2019.
-   [Miscellaneous](https://github.com/setzler/EconData/tree/master/DataRepo/Miscellaneous/)
    cross-walks, distances, and industry classifications.
