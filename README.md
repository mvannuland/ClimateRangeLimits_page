# DS_Project_2

## Predicting species climate range limits

**Description:** This project shows how to combine quantile regressions with plant trait data and climate variables to better understand species geographic ranges. Data are from Van Nuland et al. (2020) "Intraspecific trait variation across elevation predicts a widespread tree species' climate niche and range limits" in <em>Ecology and Evolution</em>.
 
Briefly, this study leveraged the natural variation across plant trait measuresments (e.g., leaf area, tree diameter) to predict where climates may be too difficult for a tree species to grow and thrive. The ecological idea behind this project is relatively straightforward: if climate stress leaves a consistent signature on plant trait variation, then trait distributions should be informative for predicting the temperature and precipitation extremes that define species range limits. Using quantile regression is helpful here because you might expect that a given trait-climate relationship could differ between the upper 95th percentile, median 50th percentile, and lower 5th percentile of the climate gradient. For example, leaf traits might respond differently to temperature extremes at the upper warm edge vs. the lower cold edge of the species climate range, and quantile regressions can be useful for teasing apart these different response patterns. 

In the study, I used an approach to sample plant traits across elevation gradients (which act as natural climate gradients) to capture the necessary variation in trait-climate relationships in order to test this idea. See the full project and results from the paper here for more information: https://doi.org/10.1002/ece3.5969.

The following code combines two datasets:

-- A .csv file of plant trait measurements (https://github.com/mvannuland/DataSciPorfolio_datasets)

-- 19 geoTiff files of climate variables (https://www.worldclim.org/data/bioclim.html)


### Contents:
**1   -** Setup

**2   -** Quantile Regressions 

**3   -** Multivariate analysis 

**4   -** Mapping climate constraints 
