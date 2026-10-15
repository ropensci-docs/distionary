# Odds Function

Access a distribution's odds function. The odds of an event having
probability `p` is `p / (1 - p)`.

## Usage

``` r
eval_odds(distribution, at)

enframe_odds(..., at, arg_name = ".arg", fn_prefix = "odds", sep = "_")
```

## Arguments

- distribution, ...:

  A distribution, or possibly multiple distributions in the case of
  `...`.

- at:

  Vector of values to evaluate the representation at.

- arg_name:

  For `enframe_`, name of the column containing the function arguments.
  Length 1 character vector.

- fn_prefix:

  For `enframe_`, name of the function to appear in the column(s).
  Length 1 character vector.

- sep:

  When `enframe`'ing more than one distribution, the character that will
  be separating the `fn_name` and the distribution name. Length 1
  character vector.

## Value

The evaluated representation in vector form (for `eval_`) with length
matching the length of `at`, and data frame or tibble form (for
`enframe_`) with number of rows matching the length of `at`. The `at`
input occupies the first column, named `.arg` by default, or the
specification in `arg_name`; the evaluated representations for each
distribution in `...` go in the subsequent columns (one column per
distribution). For a single distribution, this column is named according
to the representation by default (cdf, survival, quantile, etc.), or the
value in `fn_prefix`. For multiple distributions, unnamed distributions
are auto-named, and columns are named
`<fn_prefix><sep><distribution_name>` (e.g., `cdf_distribution1`).

## See also

Other distributional representations:
[`eval_cdf()`](https://docs.ropensci.org/distionary/reference/cdf.md),
[`eval_chf()`](https://docs.ropensci.org/distionary/reference/chf.md),
[`eval_density()`](https://docs.ropensci.org/distionary/reference/density.md),
[`eval_hazard()`](https://docs.ropensci.org/distionary/reference/hazard.md),
[`eval_pmf()`](https://docs.ropensci.org/distionary/reference/pmf.md),
[`eval_quantile()`](https://docs.ropensci.org/distionary/reference/quantile.md),
[`eval_return()`](https://docs.ropensci.org/distionary/reference/return.md),
[`eval_survival()`](https://docs.ropensci.org/distionary/reference/survival.md)

## Examples

``` r
d <- dst_pois(1)
eval_pmf(d, at = c(1, 2, 2.5))
#> [1] 0.3678794 0.1839397 0.0000000
eval_odds(d, at = c(1, 2, 2.5))
#> [1] 0.5819767 0.2253997 0.0000000
enframe_odds(d, at = 0:4)
#> # A tibble: 5 × 2
#>    .arg   odds
#>   <int>  <dbl>
#> 1     0 0.582 
#> 2     1 0.582 
#> 3     2 0.225 
#> 4     3 0.0653
#> 5     4 0.0156
```
