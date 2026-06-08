This bundle contains updated teaching material for a 2--3 hour practical session on data representation with R.

## Files

1. `01_Introduction_Data_Representation_R.Rmd`  
   Principles, session structure, package setup, why visualisation matters, and the grammar of graphics.

2. `02_Univariate_Bivariate_Data_Representation_R.Rmd`  
   Bar charts, histograms, density plots, boxplots, scatterplots, grouped data and time series.

3. `03_Multivariate_Maps_Models_Data_Representation_R.Rmd`  
   Multiple aesthetics, faceting, summaries, uncertainty intervals, time series, maps and model displays.

4. `04_Specialist_Graphs_Data_Representation_R.Rmd`  
   Bubble charts, heatmaps, scatterplot matrices, PCA biplots, patchwork, interactive plots and exporting.

## Main package datasets

- `palmerpenguins::penguins`
- `datasauRus::datasaurus_dozen`
- `gapminder::gapminder`
- `ggplot2::mpg`
- `ggplot2::economics`

## Package installation

Run once before the practical:

```r
install.packages(c(
  "tidyverse", "palmerpenguins", "gapminder", "datasauRus",
  "patchwork", "scales", "viridis", "maps", "GGally", "plotly"
))
```
