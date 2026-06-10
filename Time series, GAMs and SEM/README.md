
This bundle contains teaching material for the final practical day on time series, Generalised Additive Models and Structural Equation Models in R. It is designed to follow the earlier sessions on data representation, GLMs, GLMMs and multivariate methods.

The session moves from recognising temporal structure, to modelling nonlinear relationships, to representing ecological systems as linked pathways. The emphasis is on practical interpretation, model checking and communicating results clearly.

## Files

1. `01_Time_Series_HTML_R.Rmd`
   Introduction to time-series data in R, including trend, seasonality, decomposition, seasonal adjustment, autocorrelation, moving averages, Holt-Winters smoothing and simple ARIMA-style forecasting.

2. `02_GAM_Introduction_HTML_R.Rmd`
   Introduction to Generalised Additive Models using simulated nonlinear data, including smooth functions, effective degrees of freedom, basis dimension `k`, smoothing penalties, model checking and comparison with linear and polynomial models.

3. `03_GAM_Practical_I_HTML_R.Rmd`
   Practical on GAMs with multiple smooth terms using `mgcv::gamSim()`, including exploratory plots, comparison with a linear model, diagnostic checking, partial prediction plots and interpretation of nonlinear covariate effects.

4. `04_GAM_Practical_II_HTML_R.Rmd`
   Practical on GAMs for ecological count data, including Poisson GAMs, offsets for sampling effort, spatial smooths using `te(x, z)`, overdispersion checks, negative-binomial GAMs and predicted abundance surfaces.

5. `05_SEM_Introduction_HTML_R.Rmd`
   Introduction to Structural Equation Models using `lavaan`, including path diagrams, direct effects, indirect effects, total effects, standardised coefficients, model fit measures, latent-variable SEM and the connection to piecewise SEM.

6. `06_SEM_Practical_HTML_R.Rmd`
   Practical SEM workflow using a simulated plant-pollinator pathway model, including component regressions, manual calculation of indirect effects, lavaan SEM syntax, model comparison, reporting guidance and optional piecewise SEM.

## Continuity added

The files include explicit links to the previous sessions:

* Session 1: time series begin with visualisation and careful description of data structure.
* GLM session: GAMs extend the GLM idea by combining link functions with smooth nonlinear effects.
* GLMM session: GAMs for count data reconnect with Poisson and negative-binomial models, offsets and grouped observations.
* Multivariate session: SEM continues the idea of systems of related variables, but shifts the focus from ordination and classification to hypothesised pathways.
* GAM Practical II links directly to ecological applications through abundance surfaces, sampling effort and spatial structure.
* SEM Practical links regression models into an ecological pathway involving environmental drivers, flowers, pollinators and seed set.


## Package installation

Run once before the practical:

```
install.packages(c(
  "tidyverse", "mgcv", "lavaan", "semPlot",
  "piecewiseSEM", "DiagrammeR", "broom"
))
```

Minimum required for the core final-day version:

```
install.packages(c(
  "tidyverse", "mgcv", "lavaan"
))
```

Optional packages:

```
install.packages(c(
  "semPlot", "piecewiseSEM", "DiagrammeR", "broom"
))
```

The optional packages are only needed for path diagrams, piecewise SEM examples and some coefficient extraction workflows.


## Important notes

For time series, the key question is:

> Are observations independent, or is there temporal structure such as trend, seasonality or autocorrelation?

For GAMs, the key question is:

> Is the relationship between the response and the covariate likely to be nonlinear?

For SEMs, the key question is:

> Are we interested in separate effects, or in a hypothesised network of ecological pathways?

## Data used

The files use built-in or simulated data so the materials are portable and reproducible.

Examples include:

* `co2`
* `AirPassengers`
* `nottem`
* simulated nonlinear GAM data
* simulated ecological count data
* simulated ecological SEM pathway data
* `HolzingerSwineford1939` from `lavaan`

## Reproducibility

All simulations use `set.seed()` so results are reproducible.

Each RMarkdown file can be knitted independently to HTML. The files do not require local `.RData` files or remote datasets.

## Final message

The final day brings together three important ideas:

* time-series methods help us recognise temporal dependence;
* GAMs help us model nonlinear ecological and environmental responses;
* SEMs help us represent systems of linked ecological pathways.

Together, these tools extend the GLM and GLMM framework into richer applied modelling workflows.

The key message for students is:

> Choose the modelling framework based on the scientific question, the response type and the structure of the data.

