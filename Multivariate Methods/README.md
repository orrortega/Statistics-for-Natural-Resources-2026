This bundle contains updated teaching material for an approximately 4--5 hour practical session on multivariate methods with R. It is designed to follow the earlier sessions on data representation, GLMs and GLMMs.

## Files

1. `01_Multivariate_Methods_Continuity_R.Rmd`  
   Session overview, continuity with previous sessions, method map, shared dataset setup, scaling and correlation structure.

2. `02_PCA_Analysis_R.Rmd`  
   PCA using `palmerpenguins`, including standardisation, scree plots, scores, loadings, biplots and a short GLM bridge using PCA scores.

3. `03_Clustering_R.Rmd`  
   K-means and hierarchical clustering using the same penguin trait data, including elbow plots, silhouette widths and interpretation against known species labels.

4. `04_Discriminant_Analysis_R.Rmd`  
   Linear discriminant analysis using `MASS::lda()`, including train-test split, discriminant-score plots, posterior probabilities and confusion matrices.

5. `05_NMDS_Ecological_Ordination_R.Rmd`  
   NMDS for ecological community data using `vegan::dune`, including Bray-Curtis dissimilarity, stress, species/site scores, environmental overlays and PERMANOVA.

6. `06_EFA_Optional_Latent_Structure_R.Rmd`  
   Optional extension on exploratory factor analysis using `psych::bfi`, including parallel analysis, rotated loadings and factor scores.

7. `07_CLMM_Ordinal_Mixed_Models_R.Rmd`  
   Optional extension connecting back to the GLMM session, using cumulative link mixed models for ordinal responses with `ordinal::wine`.

## Package installation

Run once before the practical:

```r
install.packages(c(
  "tidyverse", "palmerpenguins", "GGally", "cluster", "MASS",
  "vegan", "psych", "GPArotation", "ordinal", "broom", "patchwork"
))
```

## Notes

The session is designed to avoid presenting multivariate methods as disconnected recipes. The core thread is:

1. Start with many variables and visualise them.
2. Use PCA to summarise continuous traits.
3. Use clustering to ask whether observations group naturally.
4. Use LDA to ask whether known groups can be separated and predicted.
5. Use NMDS to move from trait tables to ecological community composition.
6. Use optional EFA or CLMM material depending on whether the module needs latent-variable or ordinal mixed-model extensions.
