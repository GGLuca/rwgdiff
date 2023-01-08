# rwgDiff Package

## Overview

Whereas high $r_{WG}$ --scores are known as a requirement for data aggregation from individuals in social entities (in particular teams) in order to justify the measurement and appropriately use higher level constructs (in particular team variables), they have been neglected to be used as a substantive measure of agreement. For example, groups might be compared whether they differ in the degree of conformity, or the strength of their social norms: the standards of acceptable behavior.

One reason for this state of affairs might be the lack of a convenient method to test the difference between $r_{WG}$ --scores, which are essentially a measure of *within-group agreement*, the degree of similarity between the ratings or evaluations given by different individuals or raters of a certain target.

This package includes several functions that allow for an easy way to test for significance when comparing the strength of rater agreement within two groups, using the steps proposed by @cohen_2001.

## Installation

``` r
devtools::install_github("GGLuca/rwgDiff")
```
## Usage

``` r
library(rwgdiff)
```

## Example

### $r_{WG}$ scores as indicators of substantial differences between social entities: e.g.: gender specific social norms.

The data stems from an online conducted pilot study that aimed to better understand reactions to violation of social norms pertaining to different situations that may arise during an employment period.

As part of the study, the participants were asked to rate their emotional reaction towards various situations, such as the following:

> When I hear that someone in my work environment is to be laid off, my first spontaneous reactions are:

Emotional reactions towards dismissals were measured using eight items, that had response categories that range from 1 (*do not agree*) to 5 (*completely agree*). An example item from the scale was "*I would understand if the person involved would take revenge*".

Let us assume that we are interested to know whether there are gender specific social norms, i.e., men and women (two distinct groups) show differences in their shared perceptions regarding their acceptance of this version of retaliatory behavior in the case of a dismissal.

For example, we could hypothesize that men differ from women (and additionally agree more on the respective issues) in their endorsement of revenge as justified because they are more aggressive in general [@archer_2004] or that they adhere to elements of a culture of honor to a greater extent [@saucier_2014].

For a single item $r_{WG}$: 

``` r
rwg.diff.ci(data, construct, grouping, variance, samples)
```

### Arguments

In general, the functions takes five arguments:

1.  `data`     : a data frame containing the data.
2.  `construct`: a string naming the column that contains the construct of interest.
3.  `grouping` : a string that indicates the group membership.
4.  `variance` : the shape of the alternative null distribution.
5.  `samples`  : the number of bootstrap replicates to be used.

### About
