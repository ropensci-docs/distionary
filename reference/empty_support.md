# The Empty Support

A support containing nothing: no atoms and no continuous part.

## Usage

``` r
empty_support()
```

## Value

A support object (class `"support"`) with both parts empty.

## Details

No distribution has an empty support — probability has to go somewhere —
and
[`distribution()`](https://docs.ropensci.org/distionary/reference/distribution.md)
rejects one. It exists so that operations on supports are *closed*:
restricting a support to a region it does not reach has to return
something, and that something is the empty support. It is also the
identity for taking unions.

Its variable type is `"empty"`, which is a different claim from
`"unknown"`. Empty says there is nowhere to place probability; unknown
says nobody specified where.

## See also

[`is_empty_support()`](https://docs.ropensci.org/distionary/reference/is_support.md)
to test for it,
[`discrete()`](https://docs.ropensci.org/distionary/reference/support-construction.md),
[`continuous()`](https://docs.ropensci.org/distionary/reference/support-construction.md),
and
[`mixed()`](https://docs.ropensci.org/distionary/reference/support-construction.md)
for supports a distribution can actually have.

Other Support:
[`atoms()`](https://docs.ropensci.org/distionary/reference/atoms.md),
[`is_support()`](https://docs.ropensci.org/distionary/reference/is_support.md),
[`support()`](https://docs.ropensci.org/distionary/reference/support.md),
[`support-construction`](https://docs.ropensci.org/distionary/reference/support-construction.md)

## Examples

``` r
empty_support()
#> <support: empty>
is_empty_support(empty_support())
#> [1] TRUE

# It is also what any of the constructors gives when handed nothing.
continuous(numeric(0))
#> <support: empty>
discrete(numeric(0))
#> <support: empty>
mixed()
#> <support: empty>
```
