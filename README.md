# Statistics for Natural Resources (2026 version)

Teaching materials for a short applied course on data representation, statistical modelling and multivariate methods in R.

**Author:** Oscar Rodriguez de Rivera Ortega, PhD
**Affiliation:** University of Exeter

## Course overview

This course introduces practical tools for exploring, visualising and modelling data in R. The materials are designed for students and researchers who want to develop applied statistical skills using reproducible RMarkdown workflows.

The course moves from exploratory data visualisation to generalised linear models, mixed models, multivariate methods, time series, generalised additive models and structural equation modelling.

The emphasis is on applied understanding: choosing suitable methods, fitting models in R, interpreting outputs and communicating results clearly.

## Learning objectives

By the end of the course, students should be able to:

* import, clean and explore data in R;
* produce clear univariate, bivariate and multivariate visualisations;
* choose appropriate plots for different data types and scientific questions;
* fit and interpret linear models, GLMs and GLMMs;
* distinguish Gaussian, binomial, Poisson and negative-binomial response distributions;
* understand link functions and response scales;
* recognise grouping, repeated measurements and pseudoreplication;
* assess overdispersion and model fit;
* use PCA, clustering, discriminant analysis and ordination methods;
* fit and interpret GAMs for nonlinear relationships;
* understand basic time-series structure;
* introduce pathway-based thinking using SEM;
* write reproducible reports using RMarkdown.

## Course structure

The course is organised into five main sessions.

### Session 1: Data representation and visualisation

Topics include:

* RMarkdown workflow;
* tidy data principles;
* univariate plots;
* bivariate plots;
* multivariate visualisation;
* faceting and aesthetics;
* maps and spatial visualisation;
* interactive and publication-quality graphics.

Example packages:

```r
tidyverse
ggplot2
palmerpenguins
gapminder
patchwork
plotly
sf
maps
```

### Session 2: Generalised linear models

Topics include:

* linear models as a foundation for GLMs;
* Gaussian GLMs;
* logistic regression;
* Poisson regression;
* model comparison using AIC;
* prediction on the response scale;
* classification thresholds;
* sensitivity and specificity;
* overdispersion;
* negative-binomial models.

Example packages:

```r
tidyverse
palmerpenguins
MASS
broom
performance
```

### Session 3: Generalised linear mixed models

Topics include:

* response distributions for GLMMs;
* grouped and repeated observations;
* complete pooling, no pooling and partial pooling;
* random intercepts;
* random slopes;
* binomial GLMMs;
* Poisson GLMMs;
* overdispersion checks;
* negative-binomial GLMMs;
* population-level and group-level predictions.

Example packages:

```r
tidyverse
lme4
ggeffects
broom.mixed
performance
DHARMa
glmmTMB
```

### Session 4: Multivariate methods

Topics include:

* multivariate data structures;
* PCA;
* clustering;
* discriminant analysis;
* NMDS and ecological ordination;
* exploratory factor analysis;
* ordinal mixed models.

Example packages:

```r
tidyverse
palmerpenguins
vegan
MASS
cluster
factoextra
ordinal
psych
```

### Session 5: Time series, GAMs and SEM

Topics include:

* basic time-series exploration;
* autocorrelation;
* trends and seasonality;
* generalised additive models;
* smooth terms;
* model-based prediction;
* structural equation modelling;
* path diagrams;
* piecewise SEM.

Example packages:

```r
tidyverse
mgcv
gratia
lavaan
semPlot
piecewiseSEM
DiagrammeR
```


## Installation

Install the core packages with:

```r
install.packages(c(
  "tidyverse",
  "rmarkdown",
  "knitr",
  "ggplot2",
  "patchwork",
  "palmerpenguins",
  "gapminder",
  "MASS",
  "lme4",
  "ggeffects",
  "broom",
  "broom.mixed",
  "performance",
  "DHARMa",
  "glmmTMB",
  "vegan",
  "cluster",
  "factoextra",
  "ordinal",
  "psych",
  "mgcv",
  "gratia",
  "lavaan",
  "semPlot",
  "piecewiseSEM",
  "DiagrammeR",
  "plotly",
  "sf",
  "maps"
))
```

Some packages may require additional system dependencies, especially spatial packages such as `sf`.

## Datasets

Most examples use built-in or package datasets to keep the course portable. Examples include:

* `palmerpenguins::penguins`;
* `gapminder::gapminder`;
* `lme4::sleepstudy`;
* `lme4::cbpp`;
* `warpbreaks`;
* `datasets::co2`;
* ecological example datasets from `vegan`.

Where simulated data are used, random seeds are set to make the examples reproducible.

## Teaching format

The structure of this course is:

| Session |                                 Topic | Suggested duration |
| ------- | ------------------------------------: | -----------------: |
| 1       | Data representation and visualisation |          2–3 hours |
| 1       |             Generalised linear models |          2–3 hours |
| 2       |       Generalised linear mixed models |            4 hours |
| 3       |                  Multivariate methods |          4–5 hours |
| 4       |             Time series, GAMs and SEM |          4–5 hours |

The timing can be adjusted depending on the level of coding experience and the amount of practical work included.

## Recommended prior knowledge

Students should ideally have basic familiarity with:

* R scripts or RMarkdown;
* data frames;
* basic plotting;
* simple linear regression;
* basic statistical terminology.

The early sessions include introductory material, so advanced R experience is not required.



## Contact

email: o.m.rodriguez-de-rivera-ortega@exeter.ac.uk
