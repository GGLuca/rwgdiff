# rwgDiff Package

# Description

Whereas high $r_{WG}$ –scores are known as a requirement for data aggregation from individuals in social entities (in particular teams) in order to justify the measurement and appropriately use higher level constructs (in particular team variables), they have been neglected to be used as a substantive measure of agreement. For example, groups might be compared whether they differ in the degree of conformity, or the strength of their social norms. One reason for this state of affairs might be the lack of a convenient method to test the difference between $r_{WG}$ –scores, which are essentially a measure of *within-group agreement*, the degree of similarity between the ratings or evaluations given by different individuals or raters of a certain target.

This package includes several functions that allow for an easy way to test for significance when comparing the strength of rater agreement of two groups.

# Usage

## Arguments

In general, the function takes five arguments:

1.  `data`: a data frame containing the data that will be used to calculate the confidence interval.
2.  `construct`: a character string specifying the name of the column that contains the construct of interest.
3.  `grouping` : a character string specifying the name of the column that indicates group membership.
4.  `variance` : a number specifying the name of the column that contains the variance of the data.
5.  `samples`: the number of bootstrap replicates to be used.

## Examples

## About