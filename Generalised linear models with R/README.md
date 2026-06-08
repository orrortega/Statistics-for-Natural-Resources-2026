This bundle contains updated teaching material for a short 1--2 hour practical session on generalised linear models with R.

## Files

1. `01_GLM_Introduction_R.Rmd`  
   GLM motivation, families, links, `glm()` syntax, prediction scales and a Gaussian GLM example.

2. `02_Logistic_Regression_R.Rmd`  
   Logistic regression for binary data using `palmerpenguins`, including probabilities, odds ratios, classification thresholds and confusion matrices.

3. `03_Poisson_GLM_R.Rmd`  
   Poisson GLMs for count data using `warpbreaks`, including prediction, overdispersion, quasi-Poisson, negative-binomial models and offsets for rates.
     

## Package installation

Run once before the practical:

```r
install.packages(c("tidyverse", "palmerpenguins", "MASS", "pROC"))
```

`pROC` is only used in an optional, non-evaluated ROC-curve extension. The main slides use `tidyverse`, `palmerpenguins` and `MASS`.
