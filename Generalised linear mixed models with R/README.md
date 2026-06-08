This bundle contains updated teaching material for an approximately 4-hour practical session on generalised linear mixed models (GLMMs) with R.

## Files

1. `01_Distributions_for_GLMMs_R.Rmd`  
   A practical recap of response types, probability distributions, link functions and overdispersion. This replaces the older `manipulate`-based distribution playground with static, portable `ggplot2` examples.

2. `02_GLMM_Introduction_R.Rmd`  
   Conceptual introduction to mixed models, partial pooling, random intercepts, random slopes and the transition from LMMs to GLMMs. Uses `lme4::sleepstudy` and a short `lme4::cbpp` example.

3. `03_GLMM_Practical_R.Rmd`  
   A full practical workflow for binomial and Poisson GLMMs using `lme4::cbpp` and `lme4::grouseticks`, including plotting, model fitting, interpretation, diagnostics, overdispersion and optional negative-binomial/`glmmTMB` extensions.


## Package installation

Run once before the practical:

```r
install.packages(c(
  "tidyverse", "lme4", "broom.mixed", "ggeffects", "performance",
  "DHARMa", "glmmTMB", "patchwork"
))
```

Minimum required for the core session:

```r
install.packages(c("tidyverse", "lme4", "ggeffects"))
```

`DHARMa`, `performance`, `glmmTMB`, `broom.mixed` and `patchwork` are useful but can be treated as extensions if installation time is limited.
