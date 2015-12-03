CRAN Task View: Empirical Finance
---------------------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><strong>Maintainer:</strong>
Dirk Eddelbuettel</td>
<td align="left"><strong>Contact:</strong>
Dirk.Eddelbuettel at R-project.org</td>
</tr>
</tbody>
</table>

This CRAN Task View contains a list of packages useful for empirical work in Finance, grouped by topic.

Besides these packages, a very wide variety of functions suitable for empirical work in Finance is provided by both the basic R system (and its set of recommended core packages), and a number of other packages on the Comprehensive R Archive Network (CRAN). Consequently, several of the other CRAN Task Views may contain suitable packages, in particular the [Econometrics](http://cran.rstudio.com/web/views/Econometrics.html), [Multivariate](http://cran.rstudio.com/web/views/Multivariate.html), [Optimization](http://cran.rstudio.com/web/views/Optimization.html), [Robust](http://cran.rstudio.com/web/views/Robust.html), [SocialSciences](http://cran.rstudio.com/web/views/SocialSciences.html) and [TimeSeries](http://cran.rstudio.com/web/views/TimeSeries.html) Task Views.

Contributions are always welcome, and encouraged. Since the start of this CRAN task view in April 2005, most contributions have arrived as email suggestions. The source file for this particular task view file now also reside in a GitHub repository (see below) so that pull requests are also possible.

**Standard regression models**

-   A detailed overview of the available regression methodologies is provided by the [Econometrics](http://cran.rstudio.com/web/views/Econometrics.html) task view. This is complemented by the [Robust](http://cran.rstudio.com/web/views/Robust.html) which focuses on more robust and resistant methods.
-   Linear models such as ordinary least squares (OLS) can be estimated by `lm()` (from by the stats package contained in the basic R distribution). Maximum Likelihood (ML) estimation can be undertaken with the standard `optim()` function. Many other suitable methods are listed in the [Optimization](http://cran.rstudio.com/web/views/Optimization.html) view. Non-linear least squares can be estimated with the `nls()` function, as well as with `nlme()` from the [nlme](http://cran.rstudio.com/web/packages/nlme/index.html) package.
-   For the linear model, a variety of regression diagnostic tests are provided by the [car](http://cran.rstudio.com/web/packages/car/index.html), [lmtest](http://cran.rstudio.com/web/packages/lmtest/index.html), [strucchange](http://cran.rstudio.com/web/packages/strucchange/index.html), [urca](http://cran.rstudio.com/web/packages/urca/index.html), and [sandwich](http://cran.rstudio.com/web/packages/sandwich/index.html) packages. The [Rcmdr](http://cran.rstudio.com/web/packages/Rcmdr/index.html) and [Zelig](http://cran.rstudio.com/web/packages/Zelig/index.html) packages provide user interfaces that may be of interest as well.

**Time series**

-   A detailed overview of tools for time series analysis can be found in the [TimeSeries](http://cran.rstudio.com/web/views/TimeSeries.html) task view. Below a brief overview of the most important methods in finance is given.
-   Classical time series functionality is provided by the `arima()` and `KalmanLike()` commands in the basic R distribution.
-   The [dse](http://cran.rstudio.com/web/packages/dse/index.html) and [timsac](http://cran.rstudio.com/web/packages/timsac/index.html) packages provide a variety of more advanced estimation methods; [fracdiff](http://cran.rstudio.com/web/packages/fracdiff/index.html) can estimate fractionally integrated series; [longmemo](http://cran.rstudio.com/web/packages/longmemo/index.html) covers related material. The [fractal](http://cran.rstudio.com/web/packages/fractal/index.html) provide fractal time series modeling functionality.
-   For volatility modeling, the standard GARCH(1,1) model can be estimated with the `garch()` function in the [tseries](http://cran.rstudio.com/web/packages/tseries/index.html) package. Rmetrics (see below) contains the [fGarch](http://cran.rstudio.com/web/packages/fGarch/index.html) package which has additional models. The [rugarch](http://cran.rstudio.com/web/packages/rugarch/index.html) package can be used to model a variety of univariate GARCH models with extensions such as ARFIMA, in-mean, external regressors and various other specifications; with methods for fit, forecast, simulation, inference and plotting are provided too. The [rmgarch](http://cran.rstudio.com/web/packages/rmgarch/index.html) builds on it to provide the ability to estimate several multivariate GARCH models. The [betategarch](http://cran.rstudio.com/web/packages/betategarch/index.html) package can estimate and simulate the Beta-t-EGARCH model by Harvey. The [bayesGARCH](http://cran.rstudio.com/web/packages/bayesGARCH/index.html) package can perform Bayesian estimation of a GARCH(1,1) model with Student's t innovations. For multivariate models, the [ccgarch](http://cran.rstudio.com/web/packages/ccgarch/index.html) package can estimate (multivariate) Conditional Correlation GARCH models whereas the [gogarch](http://cran.rstudio.com/web/packages/gogarch/index.html) package provides functions for generalized orthogonal GARCH models. The [gets](http://cran.rstudio.com/web/packages/gets/index.html) package (which was preceded by a related package AutoSEARCH) provides automated general-to-specific model selection of the mean and log-volatility of a log-ARCH-X model. The [GEVStableGarch](http://cran.rstudio.com/web/packages/GEVStableGarch/index.html) package can fit ARMA-GARCH or ARMA-APARCH models with GEV and stable conditional distributions. The [lgarch](http://cran.rstudio.com/web/packages/lgarch/index.html) package can estimate and fit log-Garch models.
-   Unit root and cointegration tests are provided by [tseries](http://cran.rstudio.com/web/packages/tseries/index.html), and [urca](http://cran.rstudio.com/web/packages/urca/index.html). The Rmetrics packages [timeSeries](http://cran.rstudio.com/web/packages/timeSeries/index.html) and [fMultivar](http://cran.rstudio.com/web/packages/fMultivar/index.html) contain a number of estimation functions for ARMA, GARCH, long memory models, unit roots and more. The [CADFtest](http://cran.rstudio.com/web/packages/CADFtest/index.html) package implements the Hansen unit root test.
-   [MSBVAR](http://cran.rstudio.com/web/packages/MSBVAR/index.html) provides Bayesian estimation of vector autoregressive models. The [dlm](http://cran.rstudio.com/web/packages/dlm/index.html) package provides Bayesian and likelihood analysis of dynamic linear models (ie linear Gaussian state space models).
-   The [vars](http://cran.rstudio.com/web/packages/vars/index.html) package offer estimation, diagnostics, forecasting and error decomposition of VAR and SVAR model in a classical framework.
-   The [dyn](http://cran.rstudio.com/web/packages/dyn/index.html) and [dynlm](http://cran.rstudio.com/web/packages/dynlm/index.html) are suitable for dynamic (linear) regression models.
-   Several packages provide wavelet analysis functionality: [rwt](http://cran.rstudio.com/web/packages/rwt/index.html), [wavelets](http://cran.rstudio.com/web/packages/wavelets/index.html), [waveslim](http://cran.rstudio.com/web/packages/waveslim/index.html), [wavethresh](http://cran.rstudio.com/web/packages/wavethresh/index.html). Some methods from chaos theory are provided by the package [tseriesChaos](http://cran.rstudio.com/web/packages/tseriesChaos/index.html). [tsDyn](http://cran.rstudio.com/web/packages/tsDyn/index.html) adds time series analysis based on dynamical systems therory.
-   The [forecast](http://cran.rstudio.com/web/packages/forecast/index.html) package adds functions for forecasting problems.
-   The [tsfa](http://cran.rstudio.com/web/packages/tsfa/index.html) package provides functions for time series factor analysis.
-   The [stochvol](http://cran.rstudio.com/web/packages/stochvol/index.html) package implements Bayesian estimation of stochastic volatility using Markov Chain Monte Carlo.

**Finance**

-   The Rmetrics suite of packages comprises [fArma](http://cran.rstudio.com/web/packages/fArma/index.html), [fAsianOptions](http://cran.rstudio.com/web/packages/fAsianOptions/index.html), [fAssets](http://cran.rstudio.com/web/packages/fAssets/index.html), [fBasics](http://cran.rstudio.com/web/packages/fBasics/index.html), [fBonds](http://cran.rstudio.com/web/packages/fBonds/index.html), [timeDate](http://cran.rstudio.com/web/packages/timeDate/index.html) (formerly: fCalendar), [fCopulae](http://cran.rstudio.com/web/packages/fCopulae/index.html), [fExoticOptions](http://cran.rstudio.com/web/packages/fExoticOptions/index.html), [fExtremes](http://cran.rstudio.com/web/packages/fExtremes/index.html), [fGarch](http://cran.rstudio.com/web/packages/fGarch/index.html), [fImport](http://cran.rstudio.com/web/packages/fImport/index.html), [fNonlinear](http://cran.rstudio.com/web/packages/fNonlinear/index.html), [fOptions](http://cran.rstudio.com/web/packages/fOptions/index.html), [fPortfolio](http://cran.rstudio.com/web/packages/fPortfolio/index.html), [fRegression](http://cran.rstudio.com/web/packages/fRegression/index.html), [timeSeries](http://cran.rstudio.com/web/packages/timeSeries/index.html) (formerly: fSeries), [fTrading](http://cran.rstudio.com/web/packages/fTrading/index.html), [fUnitRoots](http://cran.rstudio.com/web/packages/fUnitRoots/index.html) and contains a very large number of relevant functions for different aspect of empirical and computational finance.
-   The [RQuantLib](http://cran.rstudio.com/web/packages/RQuantLib/index.html) package provides several option-pricing functions as well as some fixed-income functionality from the QuantLib project to R.
-   The [quantmod](http://cran.rstudio.com/web/packages/quantmod/index.html) package offers a number of functions for quantitative modelling in finance as well as data acqusition, plotting and other utilities.
-   The [portfolio](http://cran.rstudio.com/web/packages/portfolio/index.html) package contains classes for equity portfolio management; the [portfolioSim](http://cran.rstudio.com/web/packages/portfolioSim/index.html) builds a related simulation framework. The [backtest](http://cran.rstudio.com/web/packages/backtest/index.html) offers tools to explore portfolio-based hypotheses about financial instruments. The [stockPortfolio](http://cran.rstudio.com/web/packages/stockPortfolio/index.html) package provides functions for single index, constant correlation and multigroup models. The [pa](http://cran.rstudio.com/web/packages/pa/index.html) package offers performance attribution functionality for equity portfolios.
-   The [PerformanceAnalytics](http://cran.rstudio.com/web/packages/PerformanceAnalytics/index.html) package contains a large number of functions for portfolio performance calculations and risk management.
-   The [TTR](http://cran.rstudio.com/web/packages/TTR/index.html) contains functions to construct technical trading rules in R.
-   The [financial](http://cran.rstudio.com/web/packages/financial/index.html) package can compute present values, cash flows and other simple finance calculations.
-   The [sde](http://cran.rstudio.com/web/packages/sde/index.html) package provides simulation and inference functionality for stochastic differential equations.
-   The [termstrc](http://cran.rstudio.com/web/packages/termstrc/index.html) and [YieldCurve](http://cran.rstudio.com/web/packages/YieldCurve/index.html) packages contain methods for the estimation of zero-coupon yield curves and spread curves based the parametric Nelson and Siegel (1987) method with the Svensson (1994) extension. The former package adds the McCulloch (1975) cubic splines approach, the latter package adds the Diebold and Li approach. The [SmithWilsonYieldCurve](http://cran.rstudio.com/web/packages/SmithWilsonYieldCurve/index.html) construct the yield curve using the Smith-Wilson approach based on LIBOR and SWAP rates.
-   The [vrtest](http://cran.rstudio.com/web/packages/vrtest/index.html) package contains a number of variance ratio tests for the weak-form of the efficient markets hypothesis.
-   The [gmm](http://cran.rstudio.com/web/packages/gmm/index.html) package provides generalized method of moments (GMM) estimations function that are often used when estimating the parameters of the moment conditions implied by an asset pricing model.
-   The [tawny](http://cran.rstudio.com/web/packages/tawny/index.html) package contains estimator based on random matrix theory as well as shrinkage methods to remove sampling noise when estimating sample covariance matrices.
-   The [opefimor](http://cran.rstudio.com/web/packages/opefimor/index.html) package by contains material to accompany the Iacus (2011) book entitled "Option Pricing and Estimation of Financial Models in R".
-   The [maRketSim](http://cran.rstudio.com/web/packages/maRketSim/index.html) package provides a market simulator, initially designed around the bond market.
-   The [BurStFin](http://cran.rstudio.com/web/packages/BurStFin/index.html) and [BurStMisc](http://cran.rstudio.com/web/packages/BurStMisc/index.html) package has a collection of function for Finance including the estimation of covariance matrices.
-   The [AmericanCallOpt](http://cran.rstudio.com/web/packages/AmericanCallOpt/index.html) package contains a pricer for different American call options.
-   The [VarSwapPrice](http://cran.rstudio.com/web/packages/VarSwapPrice/index.html) package can price a variance swap via a portfolio of European options contracts.
-   The [FinAsym](http://cran.rstudio.com/web/packages/FinAsym/index.html) package implements the Lee and Ready (1991) and Easley and O'Hara (1987) tests for, respectively, trade direction, and probability of informed trading.
-   The [parma](http://cran.rstudio.com/web/packages/parma/index.html) package provides support for portfolio allocation and risk management applications.
-   The [GUIDE](http://cran.rstudio.com/web/packages/GUIDE/index.html) package provides a *GUI* for *DE* rivatives and contains numerous pricer examples as well as interactive 2d and 3d plots to study these pricing functions.
-   The [SharpeR](http://cran.rstudio.com/web/packages/SharpeR/index.html) package contains a collection of tools for analyzing significance of trading strategies, based on the Sharpe ratio and overfit of the same.
-   The [RND](http://cran.rstudio.com/web/packages/RND/index.html) package implements various functions to extract risk-neutral densities from option prices.
-   [LSMonteCarlo](http://cran.rstudio.com/web/packages/LSMonteCarlo/index.html) can price American Options via the Least Squares Monte Carlo method
-   The [BenfordTests](http://cran.rstudio.com/web/packages/BenfordTests/index.html) package provides seven statistical tests and support functions for determining if numerical data could conform to Benford's law.
-   The [OptHedging](http://cran.rstudio.com/web/packages/OptHedging/index.html) package values call and put option portfolio and implements an optimal hedging strategy.
-   The [markovchain](http://cran.rstudio.com/web/packages/markovchain/index.html) package provides functionality to easily handle and analyse discrete Markov chains.
-   The [ycinterextra](http://cran.rstudio.com/web/packages/ycinterextra/index.html) package models yield curve interpolation and extrapolation using via the Nelson-Siegel, Svensson, or Smith-Wilson models, as well as Hermite cubic splines.
-   The [tvm](http://cran.rstudio.com/web/packages/tvm/index.html) package models provides functions for time value of money such as cashflows and yield curves.
-   The [MarkowitzR](http://cran.rstudio.com/web/packages/MarkowitzR/index.html) package provides functions to test the statistical signicance of Markowitz portfolios.
-   The [egcm](http://cran.rstudio.com/web/packages/egcm/index.html) package implements the Engle-Granger two-stage cointegration modeling procedure with a particular focus on pairs trading.
-   The [pbo](http://cran.rstudio.com/web/packages/pbo/index.html) package models the probability of backtest overfitting, performance degradation, probability of loss, and the stochastic dominance when analysing trading strategies.
-   The [OptionPricing](http://cran.rstudio.com/web/packages/OptionPricing/index.html) package implements efficient Monte Carlo algorithms for the price and the sensitivities of Asian and European Options under Geometric Brownian Motion.
-   The [matchingMarkets](http://cran.rstudio.com/web/packages/matchingMarkets/index.html) package implements a structural estimator to correct for the bias arising from endogenous matching (e.g. group formation in microfinance or matching of firms and venture capitalists).
-   The [restimizeapi](http://cran.rstudio.com/web/packages/restimizeapi/index.html) package interfaces the API at www.estimize.com which provides crowd-sourced earnings estimates.
-   The [credule](http://cran.rstudio.com/web/packages/credule/index.html) package is another pricer for credit default swaps.
-   The [covmat](http://cran.rstudio.com/web/packages/covmat/index.html) package provides several different methods for computing covariance matrices.
-   The [PortfolioEffectHFT](http://cran.rstudio.com/web/packages/PortfolioEffectHFT/index.html) package provides portfolio analysis suitable for intra-day and high-frequency data, and also interfaces the PortfolioEffect service.

**Risk management**

-   Several packages provide functionality for Extreme Value Theory models: [evd](http://cran.rstudio.com/web/packages/evd/index.html), [evdbayes](http://cran.rstudio.com/web/packages/evdbayes/index.html), [evir](http://cran.rstudio.com/web/packages/evir/index.html), [extRemes](http://cran.rstudio.com/web/packages/extRemes/index.html), [ismev](http://cran.rstudio.com/web/packages/ismev/index.html).
-   The packages [CreditMetrics](http://cran.rstudio.com/web/packages/CreditMetrics/index.html) and [crp.CSFP](http://cran.rstudio.com/web/packages/crp.CSFP/index.html) provide function for modelling credit risks.
-   The [mvtnorm](http://cran.rstudio.com/web/packages/mvtnorm/index.html) package provides code for multivariate Normal and t-distributions.
-   The Rmetrics packages [fPortfolio](http://cran.rstudio.com/web/packages/fPortfolio/index.html) and [fExtremes](http://cran.rstudio.com/web/packages/fExtremes/index.html) also contain a number of relevant functions.
-   The [copula](http://cran.rstudio.com/web/packages/copula/index.html) and [fgac](http://cran.rstudio.com/web/packages/fgac/index.html) packages cover multivariate dependency structures using copula methods.
-   The [actuar](http://cran.rstudio.com/web/packages/actuar/index.html) package provides an actuarial perspective to risk management.
-   The [ghyp](http://cran.rstudio.com/web/packages/ghyp/index.html) package provides generalized hyberbolic distribution functions as well as procedures for VaR, CVaR or target-return portfolio optimizations.
-   The [ChainLadder](http://cran.rstudio.com/web/packages/ChainLadder/index.html) package provides functions for modeling insurance claim reserves; and the [lifecontingencies](http://cran.rstudio.com/web/packages/lifecontingencies/index.html) package provides functions for financial and actuarial evaluations of life contingencies.
-   The [frmqa](http://cran.rstudio.com/web/packages/frmqa/index.html) package aims to collect functions for Financial Risk Management and Quantitative Analysis.
-   The [ESG](http://cran.rstudio.com/web/packages/ESG/index.html) package can be used to model for asset projection, a scenario-based simulation approach.
-   The [riskSimul](http://cran.rstudio.com/web/packages/riskSimul/index.html) package provides efficient simulation procedures to estimate tail loss probabilities and conditional excess for a stock portfolios where log-returns are assumed to follow a t-copula model with generalized hyperbolic or t marginals.
-   The [GCPM](http://cran.rstudio.com/web/packages/GCPM/index.html) package anlyzes the default risk of credit portfolio using both analytical and simulation approaches.
-   The [FatTailsR](http://cran.rstudio.com/web/packages/FatTailsR/index.html) package provides a family of four distributions tailored to distribution with symmetric and asymmetric fat tails.
-   The [PortRisk](http://cran.rstudio.com/web/packages/PortRisk/index.html) computes portfolio risk attribution.

**Books**

-   The [FinTS](http://cran.rstudio.com/web/packages/FinTS/index.html) package provides an R companion to Tsay (2005), *Analysis of Financial Time Series* , 2nd ed. Wiley, and includes data sets, functions and script files to work some of the examples.
-   The [NMOF](http://cran.rstudio.com/web/packages/NMOF/index.html) package provides functions, examples and data from *Numerical Methods in Finance* by Manfred Gilli, Dietmar Maringer and Enrico Schumann (2011), including the different optimization heuristics such as Differential Evolution, Genetic Algorithms, Particle Swarms, and Threshold Accepting.
-   The [FRAPO](http://cran.rstudio.com/web/packages/FRAPO/index.html) package provides data sets and code for the book *Financial Risk Modelling and Portfolio Optimization with R* by Bernhard Paff (2013).

**Data and date management**

-   The [its](http://cran.rstudio.com/web/packages/its/index.html), [zoo](http://cran.rstudio.com/web/packages/zoo/index.html) and [timeDate](http://cran.rstudio.com/web/packages/timeDate/index.html) (part of Rmetrics) packages provide support for irregularly-spaced time series. The [xts](http://cran.rstudio.com/web/packages/xts/index.html) package extends [zoo](http://cran.rstudio.com/web/packages/zoo/index.html) specifically for financial time series. See the [TimeSeries](http://cran.rstudio.com/web/views/TimeSeries.html) task view for more details.
-   [timeDate](http://cran.rstudio.com/web/packages/timeDate/index.html) also addresses calendar issues such as recurring holidays for a large number of financial centers, and provides code for high-frequency data sets.
-   The [fame](http://cran.rstudio.com/web/packages/fame/index.html) package can access Fame time series databases (but also requires a Fame backend). The [tis](http://cran.rstudio.com/web/packages/tis/index.html) package provides time indices and time-indexed series compatible with Fame frequencies.
-   The [TSdbi](http://cran.rstudio.com/web/packages/TSdbi/index.html) package provides a unifying interface for several time series data base backends, and its SQL implementations provide a database table design.
-   The [IBrokers](http://cran.rstudio.com/web/packages/IBrokers/index.html) package provides access to the Interactive Brokers API for data access (but requires an account to access the service).
-   The [data.table](http://cran.rstudio.com/web/packages/data.table/index.html) package provides very efficient and fast access to in-memory data sets such as asset prices.
-   The [TFX](http://cran.rstudio.com/web/packages/TFX/index.html) package provides an interface to the TrueFX (TM) service for free streaming real-time and historical tick-by-tick market data for interbank foreign exchange rates at the millisecond resolution.
-   The package [highfrequency](http://cran.rstudio.com/web/packages/highfrequency/index.html) contains functionality to manage, clean and match highfrequency trades and quotes data and enables users to calculate various liquidity measures, estimate and forecast volatility, and investigate microstructure noise and intraday periodicity.
-   The [Rbitcoin](http://cran.rstudio.com/web/packages/Rbitcoin/index.html) package offers access to Bitcoin exchange APIs (mtgox, bitstamp, btce, kraken) via public and private API calls and integration of data structures for all markets.
-   The [bizdays](http://cran.rstudio.com/web/packages/bizdays/index.html) package compute business days if provided a list of holidays.
-   The [TAQMNGR](http://cran.rstudio.com/web/packages/TAQMNGR/index.html) package manages tick-by-tick (equity) transaction data performing 'cleaning', 'aggregation' and 'import' where cleaning and aggregation are performed according to Brownlees and Gallo (2006).
-   The [Rblpapi](http://cran.rstudio.com/web/packages/Rblpapi/index.html) offers efficient access to the Bloomberg API and allows `bdp`, `bdh`, and `bds` queries as well as data retrieval both in (regular time-)bars and ticks (albeit without subsecond resolution).

### CRAN packages:

-   [actuar](http://cran.rstudio.com/web/packages/actuar/index.html)
-   [AmericanCallOpt](http://cran.rstudio.com/web/packages/AmericanCallOpt/index.html)
-   [backtest](http://cran.rstudio.com/web/packages/backtest/index.html)
-   [bayesGARCH](http://cran.rstudio.com/web/packages/bayesGARCH/index.html)
-   [BenfordTests](http://cran.rstudio.com/web/packages/BenfordTests/index.html)
-   [betategarch](http://cran.rstudio.com/web/packages/betategarch/index.html)
-   [bizdays](http://cran.rstudio.com/web/packages/bizdays/index.html)
-   [BurStFin](http://cran.rstudio.com/web/packages/BurStFin/index.html)
-   [BurStMisc](http://cran.rstudio.com/web/packages/BurStMisc/index.html)
-   [CADFtest](http://cran.rstudio.com/web/packages/CADFtest/index.html)
-   [car](http://cran.rstudio.com/web/packages/car/index.html)
-   [ccgarch](http://cran.rstudio.com/web/packages/ccgarch/index.html)
-   [ChainLadder](http://cran.rstudio.com/web/packages/ChainLadder/index.html)
-   [copula](http://cran.rstudio.com/web/packages/copula/index.html)
-   [covmat](http://cran.rstudio.com/web/packages/covmat/index.html)
-   [CreditMetrics](http://cran.rstudio.com/web/packages/CreditMetrics/index.html)
-   [credule](http://cran.rstudio.com/web/packages/credule/index.html)
-   [crp.CSFP](http://cran.rstudio.com/web/packages/crp.CSFP/index.html)
-   [data.table](http://cran.rstudio.com/web/packages/data.table/index.html)
-   [dlm](http://cran.rstudio.com/web/packages/dlm/index.html)
-   [dse](http://cran.rstudio.com/web/packages/dse/index.html)
-   [dyn](http://cran.rstudio.com/web/packages/dyn/index.html)
-   [dynlm](http://cran.rstudio.com/web/packages/dynlm/index.html)
-   [egcm](http://cran.rstudio.com/web/packages/egcm/index.html)
-   [ESG](http://cran.rstudio.com/web/packages/ESG/index.html)
-   [evd](http://cran.rstudio.com/web/packages/evd/index.html)
-   [evdbayes](http://cran.rstudio.com/web/packages/evdbayes/index.html)
-   [evir](http://cran.rstudio.com/web/packages/evir/index.html)
-   [extRemes](http://cran.rstudio.com/web/packages/extRemes/index.html)
-   [fame](http://cran.rstudio.com/web/packages/fame/index.html)
-   [fArma](http://cran.rstudio.com/web/packages/fArma/index.html) (core)
-   [fAsianOptions](http://cran.rstudio.com/web/packages/fAsianOptions/index.html) (core)
-   [fAssets](http://cran.rstudio.com/web/packages/fAssets/index.html) (core)
-   [FatTailsR](http://cran.rstudio.com/web/packages/FatTailsR/index.html)
-   [fBasics](http://cran.rstudio.com/web/packages/fBasics/index.html) (core)
-   [fBonds](http://cran.rstudio.com/web/packages/fBonds/index.html) (core)
-   [fCopulae](http://cran.rstudio.com/web/packages/fCopulae/index.html) (core)
-   [fExoticOptions](http://cran.rstudio.com/web/packages/fExoticOptions/index.html) (core)
-   [fExtremes](http://cran.rstudio.com/web/packages/fExtremes/index.html) (core)
-   [fgac](http://cran.rstudio.com/web/packages/fgac/index.html)
-   [fGarch](http://cran.rstudio.com/web/packages/fGarch/index.html) (core)
-   [fImport](http://cran.rstudio.com/web/packages/fImport/index.html) (core)
-   [financial](http://cran.rstudio.com/web/packages/financial/index.html)
-   [FinAsym](http://cran.rstudio.com/web/packages/FinAsym/index.html)
-   [FinTS](http://cran.rstudio.com/web/packages/FinTS/index.html)
-   [fMultivar](http://cran.rstudio.com/web/packages/fMultivar/index.html) (core)
-   [fNonlinear](http://cran.rstudio.com/web/packages/fNonlinear/index.html) (core)
-   [fOptions](http://cran.rstudio.com/web/packages/fOptions/index.html) (core)
-   [forecast](http://cran.rstudio.com/web/packages/forecast/index.html)
-   [fPortfolio](http://cran.rstudio.com/web/packages/fPortfolio/index.html) (core)
-   [fracdiff](http://cran.rstudio.com/web/packages/fracdiff/index.html)
-   [fractal](http://cran.rstudio.com/web/packages/fractal/index.html)
-   [fRegression](http://cran.rstudio.com/web/packages/fRegression/index.html) (core)
-   [frmqa](http://cran.rstudio.com/web/packages/frmqa/index.html)
-   [fTrading](http://cran.rstudio.com/web/packages/fTrading/index.html) (core)
-   [fUnitRoots](http://cran.rstudio.com/web/packages/fUnitRoots/index.html) (core)
-   [GCPM](http://cran.rstudio.com/web/packages/GCPM/index.html)
-   [gets](http://cran.rstudio.com/web/packages/gets/index.html)
-   [GEVStableGarch](http://cran.rstudio.com/web/packages/GEVStableGarch/index.html)
-   [ghyp](http://cran.rstudio.com/web/packages/ghyp/index.html)
-   [gmm](http://cran.rstudio.com/web/packages/gmm/index.html)
-   [gogarch](http://cran.rstudio.com/web/packages/gogarch/index.html)
-   [GUIDE](http://cran.rstudio.com/web/packages/GUIDE/index.html)
-   [highfrequency](http://cran.rstudio.com/web/packages/highfrequency/index.html)
-   [IBrokers](http://cran.rstudio.com/web/packages/IBrokers/index.html)
-   [ismev](http://cran.rstudio.com/web/packages/ismev/index.html)
-   [its](http://cran.rstudio.com/web/packages/its/index.html)
-   [lgarch](http://cran.rstudio.com/web/packages/lgarch/index.html)
-   [lifecontingencies](http://cran.rstudio.com/web/packages/lifecontingencies/index.html)
-   [lmtest](http://cran.rstudio.com/web/packages/lmtest/index.html)
-   [longmemo](http://cran.rstudio.com/web/packages/longmemo/index.html)
-   [LSMonteCarlo](http://cran.rstudio.com/web/packages/LSMonteCarlo/index.html)
-   [maRketSim](http://cran.rstudio.com/web/packages/maRketSim/index.html)
-   [markovchain](http://cran.rstudio.com/web/packages/markovchain/index.html)
-   [MarkowitzR](http://cran.rstudio.com/web/packages/MarkowitzR/index.html)
-   [matchingMarkets](http://cran.rstudio.com/web/packages/matchingMarkets/index.html)
-   [MSBVAR](http://cran.rstudio.com/web/packages/MSBVAR/index.html)
-   [mvtnorm](http://cran.rstudio.com/web/packages/mvtnorm/index.html)
-   [nlme](http://cran.rstudio.com/web/packages/nlme/index.html)
-   [NMOF](http://cran.rstudio.com/web/packages/NMOF/index.html)
-   [opefimor](http://cran.rstudio.com/web/packages/opefimor/index.html)
-   [OptHedging](http://cran.rstudio.com/web/packages/OptHedging/index.html)
-   [OptionPricing](http://cran.rstudio.com/web/packages/OptionPricing/index.html)
-   [pa](http://cran.rstudio.com/web/packages/pa/index.html)
-   [parma](http://cran.rstudio.com/web/packages/parma/index.html)
-   [pbo](http://cran.rstudio.com/web/packages/pbo/index.html)
-   [PerformanceAnalytics](http://cran.rstudio.com/web/packages/PerformanceAnalytics/index.html) (core)
-   [portfolio](http://cran.rstudio.com/web/packages/portfolio/index.html)
-   [portfolioSim](http://cran.rstudio.com/web/packages/portfolioSim/index.html)
-   [PortRisk](http://cran.rstudio.com/web/packages/PortRisk/index.html)
-   [quantmod](http://cran.rstudio.com/web/packages/quantmod/index.html)
-   [Rbitcoin](http://cran.rstudio.com/web/packages/Rbitcoin/index.html)
-   [Rblpapi](http://cran.rstudio.com/web/packages/Rblpapi/index.html)
-   [Rcmdr](http://cran.rstudio.com/web/packages/Rcmdr/index.html)
-   [restimizeapi](http://cran.rstudio.com/web/packages/restimizeapi/index.html)
-   [riskSimul](http://cran.rstudio.com/web/packages/riskSimul/index.html)
-   [rmgarch](http://cran.rstudio.com/web/packages/rmgarch/index.html)
-   [RND](http://cran.rstudio.com/web/packages/RND/index.html)
-   [RQuantLib](http://cran.rstudio.com/web/packages/RQuantLib/index.html)
-   [rugarch](http://cran.rstudio.com/web/packages/rugarch/index.html)
-   [rwt](http://cran.rstudio.com/web/packages/rwt/index.html)
-   [sandwich](http://cran.rstudio.com/web/packages/sandwich/index.html)
-   [sde](http://cran.rstudio.com/web/packages/sde/index.html)
-   [SharpeR](http://cran.rstudio.com/web/packages/SharpeR/index.html)
-   [SmithWilsonYieldCurve](http://cran.rstudio.com/web/packages/SmithWilsonYieldCurve/index.html)
-   [stochvol](http://cran.rstudio.com/web/packages/stochvol/index.html)
-   [stockPortfolio](http://cran.rstudio.com/web/packages/stockPortfolio/index.html)
-   [strucchange](http://cran.rstudio.com/web/packages/strucchange/index.html)
-   [TAQMNGR](http://cran.rstudio.com/web/packages/TAQMNGR/index.html)
-   [tawny](http://cran.rstudio.com/web/packages/tawny/index.html)
-   [termstrc](http://cran.rstudio.com/web/packages/termstrc/index.html)
-   [TFX](http://cran.rstudio.com/web/packages/TFX/index.html)
-   [timeDate](http://cran.rstudio.com/web/packages/timeDate/index.html) (core)
-   [timeSeries](http://cran.rstudio.com/web/packages/timeSeries/index.html) (core)
-   [timsac](http://cran.rstudio.com/web/packages/timsac/index.html)
-   [tis](http://cran.rstudio.com/web/packages/tis/index.html)
-   [TSdbi](http://cran.rstudio.com/web/packages/TSdbi/index.html)
-   [tsDyn](http://cran.rstudio.com/web/packages/tsDyn/index.html)
-   [tseries](http://cran.rstudio.com/web/packages/tseries/index.html) (core)
-   [tseriesChaos](http://cran.rstudio.com/web/packages/tseriesChaos/index.html)
-   [tsfa](http://cran.rstudio.com/web/packages/tsfa/index.html)
-   [TTR](http://cran.rstudio.com/web/packages/TTR/index.html)
-   [tvm](http://cran.rstudio.com/web/packages/tvm/index.html)
-   [urca](http://cran.rstudio.com/web/packages/urca/index.html) (core)
-   [vars](http://cran.rstudio.com/web/packages/vars/index.html)
-   [VarSwapPrice](http://cran.rstudio.com/web/packages/VarSwapPrice/index.html)
-   [vrtest](http://cran.rstudio.com/web/packages/vrtest/index.html)
-   [wavelets](http://cran.rstudio.com/web/packages/wavelets/index.html)
-   [waveslim](http://cran.rstudio.com/web/packages/waveslim/index.html)
-   [wavethresh](http://cran.rstudio.com/web/packages/wavethresh/index.html)
-   [xts](http://cran.rstudio.com/web/packages/xts/index.html) (core)
-   [ycinterextra](http://cran.rstudio.com/web/packages/ycinterextra/index.html)
-   [YieldCurve](http://cran.rstudio.com/web/packages/YieldCurve/index.html)
-   [Zelig](http://cran.rstudio.com/web/packages/Zelig/index.html)
-   [zoo](http://cran.rstudio.com/web/packages/zoo/index.html) (core)

### Related links:

-   CRAN Task View: [Econometrics](Econometrics.html)
-   CRAN Task View: [Multivariate](Multivariate.html)
-   CRAN Task View: [Optimization](Optimization.html)
-   CRAN Task View: [Robust](Robust.html)
-   CRAN Task View: [SocialSciences](SocialSciences.html)
-   CRAN Task View: [TimeSeries](TimeSeries.html)
-   [Rmetrics contains a wealth of R code for Finance](http://www.rmetrics.org)
-   [Quantlib is a C++ library for quantitative finance](http://www.quantlib.org)
-   [Documentation for the Bloomberg API accessed by Rblpapi](http://www.bloomberglabs.com//)
-   [Mailing list: R Special Interest Group Finance](https://stat.ethz.ch/mailman/listinfo/R-SIG-Finance/)
-   [MSCI indexes data](http://www.msci.com/)
-   [French/Fama data](http://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)
-   [Wilshire indexes data](http://www.wilshire.com/Indexes/calculator/)
-   [Rene Carmona](http://orfe.princeton.edu/~rcarmona/maindownload.html)
-   [Eric Zivot](http://faculty.washington.edu/ezivot/splus.htm)
-   [R Code for Ruppert's 'Statistics and Finance'](http://christopherggreen.github.io/RuppertStatisticsFinance2004/)
-   [Guy Yollin](http://www.r-programming.org/papers)
-   [GitHub repository for this Task View](https://github.com/eddelbuettel/ctv-finance)
