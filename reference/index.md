# Package index

## Specify

### Built-in Distribution Families

- [`dst_bern()`](https://docs.ropensci.org/distionary/reference/dst_bern.md)
  : Bernoulli Distribution
- [`dst_beta()`](https://docs.ropensci.org/distionary/reference/dst_beta.md)
  : Beta Distribution
- [`dst_binom()`](https://docs.ropensci.org/distionary/reference/dst_binom.md)
  : Binomial Distribution
- [`dst_cauchy()`](https://docs.ropensci.org/distionary/reference/dst_cauchy.md)
  : Cauchy Distribution
- [`dst_chisq()`](https://docs.ropensci.org/distionary/reference/dst_chisq.md)
  : Chi-Squared Distribution
- [`dst_degenerate()`](https://docs.ropensci.org/distionary/reference/dst_degenerate.md)
  : Degenerate Distribution
- [`dst_empirical()`](https://docs.ropensci.org/distionary/reference/dst_empirical.md)
  : Empirical Distribution
- [`dst_exp()`](https://docs.ropensci.org/distionary/reference/dst_exp.md)
  : Exponential Distribution
- [`dst_f()`](https://docs.ropensci.org/distionary/reference/dst_f.md) :
  F Distribution
- [`dst_finite()`](https://docs.ropensci.org/distionary/reference/dst_finite.md)
  : Finite Distribution
- [`dst_gamma()`](https://docs.ropensci.org/distionary/reference/dst_gamma.md)
  : Gamma Distribution
- [`dst_geom()`](https://docs.ropensci.org/distionary/reference/dst_geom.md)
  : Geometric Distribution
- [`dst_gev()`](https://docs.ropensci.org/distionary/reference/dst_gev.md)
  : Generalised Extreme Value Distribution
- [`dst_gp()`](https://docs.ropensci.org/distionary/reference/dst_gp.md)
  : Generalised Pareto Distribution
- [`dst_gumbel()`](https://docs.ropensci.org/distionary/reference/dst_gumbel.md)
  : Gumbel Distribution
- [`dst_hyper()`](https://docs.ropensci.org/distionary/reference/dst_hyper.md)
  : Hypergeometric Distribution
- [`dst_lnorm()`](https://docs.ropensci.org/distionary/reference/dst_lnorm.md)
  : Log Normal Distribution
- [`dst_lp3()`](https://docs.ropensci.org/distionary/reference/dst_lp3.md)
  : Log Pearson Type III distribution
- [`dst_nbinom()`](https://docs.ropensci.org/distionary/reference/dst_nbinom.md)
  : Negative binomial Distribution
- [`dst_norm()`](https://docs.ropensci.org/distionary/reference/dst_norm.md)
  : Normal (Gaussian) Distribution
- [`dst_null()`](https://docs.ropensci.org/distionary/reference/dst_null.md)
  : Null Distribution
- [`dst_pearson3()`](https://docs.ropensci.org/distionary/reference/dst_pearson3.md)
  : Pearson Type III distribution
- [`dst_pois()`](https://docs.ropensci.org/distionary/reference/dst_pois.md)
  : Poisson Distribution
- [`dst_t()`](https://docs.ropensci.org/distionary/reference/dst_t.md) :
  Student t Distribution
- [`dst_unif()`](https://docs.ropensci.org/distionary/reference/dst_unif.md)
  : Uniform Distribution
- [`dst_weibull()`](https://docs.ropensci.org/distionary/reference/dst_weibull.md)
  : Weibull Distribution

### General Distribution Creation

- [`distribution()`](https://docs.ropensci.org/distionary/reference/distribution.md)
  [`is_distribution()`](https://docs.ropensci.org/distionary/reference/distribution.md)
  [`is.distribution()`](https://docs.ropensci.org/distionary/reference/distribution.md)
  : Build a Distribution Object

### Distribution Characteristics

- [`parameters()`](https://docs.ropensci.org/distionary/reference/parameters.md)
  [`` `parameters<-`() ``](https://docs.ropensci.org/distionary/reference/parameters.md)
  : Parameters of a Distribution
- [`plot(`*`<dst>`*`)`](https://docs.ropensci.org/distionary/reference/plot.dst.md)
  : Plot a Distribution
- [`pretty_name()`](https://docs.ropensci.org/distionary/reference/pretty_name.md)
  : Distribution name
- [`vtype()`](https://docs.ropensci.org/distionary/reference/vtype.md) :
  Variable Type of a Distribution

## Evaluate

### Distributional Representations

- [`eval_cdf()`](https://docs.ropensci.org/distionary/reference/cdf.md)
  [`enframe_cdf()`](https://docs.ropensci.org/distionary/reference/cdf.md)
  : Cumulative Distribution Function
- [`eval_chf()`](https://docs.ropensci.org/distionary/reference/chf.md)
  [`enframe_chf()`](https://docs.ropensci.org/distionary/reference/chf.md)
  : Cumulative Hazard Function
- [`eval_density()`](https://docs.ropensci.org/distionary/reference/density.md)
  [`enframe_density()`](https://docs.ropensci.org/distionary/reference/density.md)
  : Probability Density Function
- [`eval_hazard()`](https://docs.ropensci.org/distionary/reference/hazard.md)
  [`enframe_hazard()`](https://docs.ropensci.org/distionary/reference/hazard.md)
  : Hazard Function
- [`eval_odds()`](https://docs.ropensci.org/distionary/reference/odds.md)
  [`enframe_odds()`](https://docs.ropensci.org/distionary/reference/odds.md)
  : Odds Function
- [`eval_pmf()`](https://docs.ropensci.org/distionary/reference/pmf.md)
  [`enframe_pmf()`](https://docs.ropensci.org/distionary/reference/pmf.md)
  : Probability Mass Function
- [`eval_quantile()`](https://docs.ropensci.org/distionary/reference/quantile.md)
  [`enframe_quantile()`](https://docs.ropensci.org/distionary/reference/quantile.md)
  : Distribution Quantiles
- [`eval_return()`](https://docs.ropensci.org/distionary/reference/return.md)
  [`enframe_return()`](https://docs.ropensci.org/distionary/reference/return.md)
  : Return Level Function
- [`eval_survival()`](https://docs.ropensci.org/distionary/reference/survival.md)
  [`enframe_survival()`](https://docs.ropensci.org/distionary/reference/survival.md)
  : Survival Function
- [`eval_property()`](https://docs.ropensci.org/distionary/reference/eval_property.md)
  : Evaluate a distribution
- [`prob_left()`](https://docs.ropensci.org/distionary/reference/flexible_cdf.md)
  [`prob_right()`](https://docs.ropensci.org/distionary/reference/flexible_cdf.md)
  : Find the probability left or right of a number

### Distribution Properties

- [`kurtosis()`](https://docs.ropensci.org/distionary/reference/moments.md)
  [`kurtosis_exc()`](https://docs.ropensci.org/distionary/reference/moments.md)
  [`mean(`*`<dst>`*`)`](https://docs.ropensci.org/distionary/reference/moments.md)
  [`skewness()`](https://docs.ropensci.org/distionary/reference/moments.md)
  [`stdev()`](https://docs.ropensci.org/distionary/reference/moments.md)
  [`variance()`](https://docs.ropensci.org/distionary/reference/moments.md)
  : Moments of a Distribution
- [`median(`*`<dst>`*`)`](https://docs.ropensci.org/distionary/reference/median.dst.md)
  : Median of a Distribution
- [`range(`*`<dst>`*`)`](https://docs.ropensci.org/distionary/reference/range.md)
  : Range of Distribution

### Random Sampling

- [`realise()`](https://docs.ropensci.org/distionary/reference/realise.md)
  [`realize()`](https://docs.ropensci.org/distionary/reference/realise.md)
  : Generate a Sample from a Distribution

### Package Overview

- [`distionary`](https://docs.ropensci.org/distionary/reference/distionary-package.md)
  [`distionary-package`](https://docs.ropensci.org/distionary/reference/distionary-package.md)
  : distionary: Create and Evaluate Probability Distributions

## Built-in Distributional Representations

Distributional representations not found in the `stats` package.

- [`dst_gev()`](https://docs.ropensci.org/distionary/reference/dst_gev.md)
  : Generalised Extreme Value Distribution
- [`pgev()`](https://docs.ropensci.org/distionary/reference/gev_raw.md)
  [`qgev()`](https://docs.ropensci.org/distionary/reference/gev_raw.md)
  [`dgev()`](https://docs.ropensci.org/distionary/reference/gev_raw.md)
  : Representations of the Generalized Extreme Value Distribution
- [`dst_gp()`](https://docs.ropensci.org/distionary/reference/dst_gp.md)
  : Generalised Pareto Distribution
- [`pgp()`](https://docs.ropensci.org/distionary/reference/gp_raw.md)
  [`qgp()`](https://docs.ropensci.org/distionary/reference/gp_raw.md)
  [`dgp()`](https://docs.ropensci.org/distionary/reference/gp_raw.md) :
  Representations of the Generalized Pareto Distribution
- [`dst_lp3()`](https://docs.ropensci.org/distionary/reference/dst_lp3.md)
  : Log Pearson Type III distribution
- [`plp3()`](https://docs.ropensci.org/distionary/reference/lp3_raw.md)
  [`dlp3()`](https://docs.ropensci.org/distionary/reference/lp3_raw.md)
  [`qlp3()`](https://docs.ropensci.org/distionary/reference/lp3_raw.md)
  [`rlp3()`](https://docs.ropensci.org/distionary/reference/lp3_raw.md)
  : Representations of the Log Pearson Type III Distribution
- [`dst_pearson3()`](https://docs.ropensci.org/distionary/reference/dst_pearson3.md)
  : Pearson Type III distribution
- [`ppearson3()`](https://docs.ropensci.org/distionary/reference/pearson3_raw.md)
  [`dpearson3()`](https://docs.ropensci.org/distionary/reference/pearson3_raw.md)
  [`qpearson3()`](https://docs.ropensci.org/distionary/reference/pearson3_raw.md)
  [`rpearson3()`](https://docs.ropensci.org/distionary/reference/pearson3_raw.md)
  : Representations of the Pearson Type III Distribution
