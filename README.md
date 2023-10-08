# rethinking2020

[![Lifecycle: stable](https://img.shields.io/badge/lifecycle-stable-brightgreen.svg)](https://lifecycle.r-lib.org/articles/stages.html) [![R 4.2.1](https://img.shields.io/badge/R-4.2.1-blueviolet.svg)](https://cran.r-project.org/bin/windows/base/)

`rethinking2020` is a study project of *Statistical Rethinking*, second edition, by Richard McElreath. [@elreath2020]

## Aknowledgement

Many thanks to Richard McElreath who wrote *Statistical Rethinking* to make Bayesian statistics so interesting.

This study project is inspired by *Solomon Kurtz* who did wonderful work. It can be found at [Solomon Kurtz](https://bookdown.org/content/3890/).

## Packages

The packages used in this project are as follows.

### Modelizations and data processing

| Package                                                                | Comment                                                                                                                                                                                      |
|-----------------------|-------------------------------------------------|
| [rethinking](https://github.com/rmcelreath/rethinking)                 | This R package accompanies a course and book on Bayesian data analysis: McElreath 2020. Statistical Rethinking, 2nd edition.                                                                 |
| [brms](https://paul-buerkner.github.io/brms/)                          | Used to do pretty much all models and computations.                                                                                                                                          |
| [loo](http://mc-stan.org/loo/index.html)                               | Used by both `rethinking` and `brms` to compute WAIC and LOO. See section 7.5 in chapter for more details.                                                                                   |
| [posterior](https://mc-stan.org/posterior/)                            | Used to work with the output of Bayesian models.                                                                                                                                             |
| [tidybayes](http://mjskay.github.io/tidybayes/articles/tidybayes.html) | Bayesian statistics do require a lot of data processing. `tidybayes` is incredibly helpful in providing a constant and efficient way of coding the data processing.                          |
| [bayestestR](https://easystats.github.io/bayestestR/)                  | A comprehensive and consistent set of functions to analyze and describe posterior distributions.                                                                                             |
| [tidyverse](https://www.tidyverse.org)                                 | **The** package for data science in general.                                                                                                                                                 |
| [extraDistr](https://github.com/twolodzko/extraDistr)                  | has many extra distributions such as BetaBinom, NegBetaBinom, HalfCauchy, ZIP, Pareto, etc. which are useful in real-world applications and usually dispersed among many different packages. |
| [ggmcmc](https://github.com/cran/ggmcmc)                               | tool for assessing and diagnosing convergence of Markov Chain Monte Carlo simulations, as well as for graphically display results from full MCMC analysis                                    |
| [simpr](https://statisfactions.github.io/simpr/)                       | tidyverse-friendly framework for generating simulated data, fitting models on simulations, and tidying model results.                                                                        |
| [modelr](https://modelr.tidyverse.org/index.html)                      | functions that help you create elegant pipelines when modelling                                                                                                                              |
| [gtools](https://github.com/r-gregmisc/gtools)                      | functions to assist in R programming, including   
`logit` and `inv.logit` functions used in many places in this project|

### Visualizations

| Package                                                 | Comment                                                                                                                                                                    |
|--------------------------|----------------------------------------------|
| [ggdist](https://mjskay.github.io/ggdist/)              | `tidybayes` relies heavily on the `ggdist` and reexport very many of it's functions. In addition `ggdist` is useful for both a frequencist as well as a bayesian approach. |
| [bayesplot](https://mc-stan.org/bayesplot/)             | Used as complement when `ggdist` and `tidybayes` do not provide a satisfactory solution.                                                                                   |
| [ggplot2](https://ggplot2.tidyverse.org)                | Vizualisations using the grammar of graphics.                                                                                                                              |
| [scales](https://scales.r-lib.org)                      | Provide the internal scaling infrastructure used by `ggplot2`                                                                                                              |
| [paletteer](https://github.com/EmilHvitfeldt/paletteer) | A nice package to manage color and shape palettes.                                                                                                                         |

### Graphs

| Package                                                                | Comment                                                           |
|--------------------------|----------------------------------------------|
| [dagitty](https://www.dagitty.net)                                     | Draw and analyse causal diagrams                                  |
| [ggdag](https://github.com/r-causal/ggdag)                             | R package to visualize and analyze causal directed acyclic graphs |
| [tidygraph](https://tidygraph.data-imaginist.com/reference/index.html) | To manipulate graph data                                          |
| [ggraph](https://ggraph.data-imaginist.com/reference/index.html)       | To visualize graphs                                               |

### Miscellaneous

| Package                                                                  | Comment                                                                                                 |
|------------------------------|------------------------------------------|
| [xfun](https://cran.r-project.org/web/packages/xfun/vignettes/xfun.html) | The function `xfun::cache_rds` is used for caching which is used several times in almost every chapter. |
