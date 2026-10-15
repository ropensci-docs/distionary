# Retrieve the Support of a Distribution

Returns the structured support of a distribution: its atomic part and
its continuous part. Every distribution has one, because
[`distribution()`](https://docs.ropensci.org/distionary/reference/distribution.md)
requires it — the single exception being
[`dst_null()`](https://docs.ropensci.org/distionary/reference/dst_null.md),
which has nothing to place anywhere and returns `NULL`.

## Usage

``` r
support(distribution)
```

## Arguments

- distribution:

  Distribution object.

## Value

A support object, or `NULL` if the distribution has no structured
support.

## See also

[`discrete()`](https://docs.ropensci.org/distionary/reference/support-construction.md),
[`continuous()`](https://docs.ropensci.org/distionary/reference/support-construction.md),
[`mixed()`](https://docs.ropensci.org/distionary/reference/support-construction.md)
to build supports;
[`vtype()`](https://docs.ropensci.org/distionary/reference/vtype.md) for
the derived variable type.

Other Support:
[`atoms()`](https://docs.ropensci.org/distionary/reference/atoms.md),
[`empty_support()`](https://docs.ropensci.org/distionary/reference/empty_support.md),
[`is_support()`](https://docs.ropensci.org/distionary/reference/is_support.md),
[`support-construction`](https://docs.ropensci.org/distionary/reference/support-construction.md)

## Examples

``` r
support(distribution(.support = continuous(c(0, Inf))))
#> Warning: Full suite of distribution properties may not be accessible without specifying 'cdf', and either 'density' or 'pmf'.
#> <support: continuous>
#> -- continuous --
#> [0, Inf]
```
