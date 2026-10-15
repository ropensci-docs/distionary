# Survival Function

Access a distribution's survival function.

## Usage

``` r
eval_survival(distribution, at)

enframe_survival(..., at, arg_name = ".arg", fn_prefix = "survival", sep = "_")
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
[`eval_odds()`](https://docs.ropensci.org/distionary/reference/odds.md),
[`eval_pmf()`](https://docs.ropensci.org/distionary/reference/pmf.md),
[`eval_quantile()`](https://docs.ropensci.org/distionary/reference/quantile.md),
[`eval_return()`](https://docs.ropensci.org/distionary/reference/return.md)

## Examples

``` r
d <- dst_unif(0, 4)
eval_survival(d, at = 0:4)
#> [1] 1.00 0.75 0.50 0.25 0.00
enframe_survival(d, at = 0:4)
#> # A tibble: 5 × 2
#>    .arg survival
#>   <int>    <dbl>
#> 1     0     1   
#> 2     1     0.75
#> 3     2     0.5 
#> 4     3     0.25
#> 5     4     0   
```
