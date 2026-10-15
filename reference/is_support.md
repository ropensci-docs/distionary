# Test for a Support Object

`is_empty_support()` tests whether a support is the empty one: no atoms
and no continuous part. It is `FALSE` for anything that is not a
support.

## Usage

``` r
is_support(x)

is_empty_support(x)
```

## Arguments

- x:

  Object to test.

## Value

`TRUE` if `x` is a support object, otherwise `FALSE`.

## See also

Other Support:
[`atoms()`](https://docs.ropensci.org/distionary/reference/atoms.md),
[`empty_support()`](https://docs.ropensci.org/distionary/reference/empty_support.md),
[`support()`](https://docs.ropensci.org/distionary/reference/support.md),
[`support-construction`](https://docs.ropensci.org/distionary/reference/support-construction.md)
