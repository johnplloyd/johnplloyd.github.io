---
layout: page
title: R packages
---

Over the years, I have written, and re-written, and forgotten about, and re-written many basic and not-so-basic functions that I use during day-to-day coding and in machine learning and model building.

To help reduce future instances of re-writing my code base, I have generated a set of R packages containing my most commonly used and useful functions.

My mantras here were flexibility and compartmentalization, with the goal of producing functions that could be called up simply and quickly to be applied to a wide variety of tasks.
&nbsp;
&nbsp;
## lloydUtils
### Lloyd's general utilities
---------

Set of general, custom R functions John often uses while coding in R.

Functions included:
```
corner
intersect.iterate
ordered_dot_plot
p_round.display
remove_outliers
transparent_color
write_df
```
&nbsp;
## lloydPerf
### Lloyd's performance calculators
---------

Set of functions for calculating performance metrics in R.

Functions included:
```
calc_AUCROC (requires package: ROCR)
calc_kappa
calc_MCC
calc_median_error
calc_MSE
calc_RSS
performance.regression
```
&nbsp;
## lloydML
### Lloyd's machine learning utilities
---------

Set of functions for building and applying statistical learning models under cross-validation or with hold-out validation sets in R.

Functions included:
```
assign_CV_folds
glmnet_feature_weights
iterate_search_lambda
multi_y.consolidate_performances
multi_y.prediction_and_performance_with_validation_set.wrapper
sort_glmnet_weights
train_and_apply_glmnet_model
train_and_apply_model
train_and_apply_under_CV
train_and_apply_with_validation_set
```
&nbsp;
## Installation
---------

Download and install [Rtools](https://cran.r-project.org/bin/windows/Rtools/) ***(required to install packages from GitHub)***

```
# install.packages("devtools")
library(devtools)

install_github("johnplloyd/R_packages/lloydUtils")
library(lloydUtils)

install_github("johnplloyd/R_packages/lloydPerf")
library(lloydPerf)

install_github("johnplloyd/R_packages/lloydML")
library(lloydML)
```
&nbsp;
