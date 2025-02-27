Historical horse population in Canada
================

-   <a href="#aim" id="toc-aim">Aim</a>
-   <a href="#data" id="toc-data">Data</a>
-   <a href="#methods" id="toc-methods">Methods</a>
-   <a href="#results" id="toc-results">Results</a>
-   <a href="#references" id="toc-references">References</a>

## Aim

This project explores the historical population of horses in Canada
between 1906 and 1972 for each Province.

## Data

Horse population data were sourced from the [Government of Canada’s Open
Data website](http://open.canada.ca/en/open-data). Specifically, these
two sources were used:

-   [Horses, number on farms at June 1 and at December
    1](http://open.canada.ca/data/en/dataset/43b3a9b3-3842-45e7-8bc8-c4c27b9462ab)
-   [Horses, number on farms at June 1, farm value per head and total
    farm
    value](http://open.canada.ca/data/en/dataset/b374f60b-9580-44dc-83f6-c0a850c15f30)

## Methods

The R programming language and the following R packages were used to
perform the analysis: knitr and tidyverse. The code used to perform the
analysis and create this report can be found here:
<https://github.com/ttimbers/equine_numbers_value_canada_rmd>.

## Results

<img src="hist_horse_pop_files/figure-gfm/plot horses-1.png" alt="Figure 1. Horse population between 1906 and 1972 in each Canadian province." width="100%" />

We can see from the visualisation above that Ontario, Saskatchewan and
Alberta have had the highest horse populations in Canada. All provinces
have had a decline in horse populations since 1940. This is likely due
to the rebound of the Canadian automotive industry after the Great
Depression and the Second World War. An interesting follow-up
visualization would be car sales per year for each Province over the
time period visualised above to further support this hypothesis.

Next we look at the range of the number horses for each provinces at any
time point between 1940 - 1972:

| Province             | Maximum | Minimum |
|:---------------------|--------:|--------:|
| Alberta              |  806200 |   87000 |
| British Columbia     |   65200 |   22500 |
| Manitoba             |  370800 |   31000 |
| New Brunswick        |   71000 |    3200 |
| Nova Scotia          |   64500 |    3600 |
| Ontario              |  822300 |   75400 |
| Prince Edward Island |   36700 |    2200 |
| Quebec               |  378800 |   39000 |
| Saskatchewan         | 1104300 |   58000 |

Table 1. Range of the number of horses for each province from 1940 to
1972.

Below we zoom in and look at the province of British Columbia:

![Figure 2. Horse population in `r params$province` between 1906 and
1972.](hist_horse_pop_files/figure-gfm/plot%20province-1.png)

The highest number of horses in British Columbia at a given time was
65,200.

## References

R Core Team (2022)

Wickham et al. (2019)

Xie (2022)

Xie (2015)

Xie (2014)

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-R" class="csl-entry">

R Core Team. 2022. *R: A Language and Environment for Statistical
Computing*. Vienna, Austria: R Foundation for Statistical Computing.
<https://www.R-project.org/>.

</div>

<div id="ref-tidyverse" class="csl-entry">

Wickham, Hadley, Mara Averick, Jennifer Bryan, Winston Chang, Lucy
D’Agostino McGowan, Romain François, Garrett Grolemund, et al. 2019.
“Welcome to the <span class="nocase">tidyverse</span>.” *Journal of Open
Source Software* 4 (43): 1686. <https://doi.org/10.21105/joss.01686>.

</div>

<div id="ref-reproducible" class="csl-entry">

Xie, Yihui. 2014. “Knitr: A Comprehensive Tool for Reproducible Research
in R.” In *Implementing Reproducible Computational Research*, edited by
Victoria Stodden, Friedrich Leisch, and Roger D. Peng. Chapman;
Hall/CRC. <http://www.crcpress.com/product/isbn/9781466561595>.

</div>

<div id="ref-dynamic" class="csl-entry">

———. 2015. *Dynamic Documents with R and Knitr*. 2nd ed. Boca Raton,
Florida: Chapman; Hall/CRC. <https://yihui.org/knitr/>.

</div>

<div id="ref-knitr" class="csl-entry">

———. 2022. *Knitr: A General-Purpose Package for Dynamic Report
Generation in r*. <https://yihui.org/knitr/>.

</div>

</div>
