CRAN Task View: Empirical Finance
---------------------------------

|                 |                                      
|-----------------|------------------------------------  
| **Maintainer:** | Dirk Eddelbuettel                    
| **Contact:**    | Dirk.Eddelbuettel at R-project.org   
| **Version:**    | 2016-05-09                           

This CRAN Task View contains a list of packages useful for empirical work in Finance, grouped by topic.

Besides these packages, a very wide variety of functions suitable for empirical work in Finance is provided by both the basic R system (and its set of recommended core packages), and a number of other packages on the Comprehensive R Archive Network (CRAN). Consequently, several of the other CRAN Task Views may contain suitable packages, in particular the [Econometrics](https://cloud.r-project.org/web/views/Econometrics.html), [Multivariate](https://cloud.r-project.org/web/views/Multivariate.html), [Optimization](https://cloud.r-project.org/web/views/Optimization.html), [Robust](https://cloud.r-project.org/web/views/Robust.html), [SocialSciences](https://cloud.r-project.org/web/views/SocialSciences.html) and [TimeSeries](https://cloud.r-project.org/web/views/TimeSeries.html) Task Views.

Contributions are always welcome, and encouraged. Since the start of this CRAN task view in April 2005, most contributions have arrived as email suggestions. The source file for this particular task view file now also reside in a GitHub repository (see below) so that pull requests are also possible.

**Standard regression models**

-   A detailed overview of the available regression methodologies is provided by the [Econometrics](https://cloud.r-project.org/web/views/Econometrics.html) task view. This is complemented by the [Robust](https://cloud.r-project.org/web/views/Robust.html) which focuses on more robust and resistant methods.
-   Linear models such as ordinary least squares (OLS) can be estimated by `lm()` (from by the stats package contained in the basic R distribution). Maximum Likelihood (ML) estimation can be undertaken with the standard `optim()` function. Many other suitable methods are listed in the [Optimization](https://cloud.r-project.org/web/views/Optimization.html) view. Non-linear least squares can be estimated with the `nls()` function, as well as with `nlme()` from the [nlme](https://cloud.r-project.org/web/packages/nlme/index.html) package.
-   For the linear model, a variety of regression diagnostic tests are provided by the [car](https://cloud.r-project.org/web/packages/car/index.html), [lmtest](https://cloud.r-project.org/web/packages/lmtest/index.html), [strucchange](https://cloud.r-project.org/web/packages/strucchange/index.html), [urca](https://cloud.r-project.org/web/packages/urca/index.html), and [sandwich](https://cloud.r-project.org/web/packages/sandwich/index.html) packages. The [Rcmdr](https://cloud.r-project.org/web/packages/Rcmdr/index.html) and [Zelig](https://cloud.r-project.org/web/packages/Zelig/index.html) packages provide user interfaces that may be of interest as well.

**Time series**

-   A detailed overview of tools for time series analysis can be found in the [TimeSeries](https://cloud.r-project.org/web/views/TimeSeries.html) task view. Below a brief overview of the most important methods in finance is given.
-   Classical time series functionality is provided by the `arima()` and `KalmanLike()` commands in the basic R distribution.
-   The [dse](https://cloud.r-project.org/web/packages/dse/index.html) and [timsac](https://cloud.r-project.org/web/packages/timsac/index.html) packages provide a variety of more advanced estimation methods; [fracdiff](https://cloud.r-project.org/web/packages/fracdiff/index.html) can estimate fractionally integrated series; [longmemo](https://cloud.r-project.org/web/packages/longmemo/index.html) covers related material. The [fractal](https://cloud.r-project.org/web/packages/fractal/index.html) provide fractal time series modeling functionality.
-   For volatility modeling, the standard GARCH(1,1) model can be estimated with the `garch()` function in the [tseries](https://cloud.r-project.org/web/packages/tseries/index.html) package. Rmetrics (see below) contains the [fGarch](https://cloud.r-project.org/web/packages/fGarch/index.html) package which has additional models. The [rugarch](https://cloud.r-project.org/web/packages/rugarch/index.html) package can be used to model a variety of univariate GARCH models with extensions such as ARFIMA, in-mean, external regressors and various other specifications; with methods for fit, forecast, simulation, inference and plotting are provided too. The [rmgarch](https://cloud.r-project.org/web/packages/rmgarch/index.html) builds on it to provide the ability to estimate several multivariate GARCH models. The [betategarch](https://cloud.r-project.org/web/packages/betategarch/index.html) package can estimate and simulate the Beta-t-EGARCH model by Harvey. The [bayesGARCH](https://cloud.r-project.org/web/packages/bayesGARCH/index.html) package can perform Bayesian estimation of a GARCH(1,1) model with Student's t innovations. For multivariate models, the [ccgarch](https://cloud.r-project.org/web/packages/ccgarch/index.html) package can estimate (multivariate) Conditional Correlation GARCH models whereas the [gogarch](https://cloud.r-project.org/web/packages/gogarch/index.html) package provides functions for generalized orthogonal GARCH models. The [gets](https://cloud.r-project.org/web/packages/gets/index.html) package (which was preceded by a related package AutoSEARCH) provides automated general-to-specific model selection of the mean and log-volatility of a log-ARCH-X model. The [GEVStableGarch](https://cloud.r-project.org/web/packages/GEVStableGarch/index.html) package can fit ARMA-GARCH or ARMA-APARCH models with GEV and stable conditional distributions. The [lgarch](https://cloud.r-project.org/web/packages/lgarch/index.html) package can estimate and fit log-Garch models.
-   Unit root and cointegration tests are provided by [tseries](https://cloud.r-project.org/web/packages/tseries/index.html), and [urca](https://cloud.r-project.org/web/packages/urca/index.html). The Rmetrics packages [timeSeries](https://cloud.r-project.org/web/packages/timeSeries/index.html) and [fMultivar](https://cloud.r-project.org/web/packages/fMultivar/index.html) contain a number of estimation functions for ARMA, GARCH, long memory models, unit roots and more. The [CADFtest](https://cloud.r-project.org/web/packages/CADFtest/index.html) package implements the Hansen unit root test.
-   [MSBVAR](https://cloud.r-project.org/web/packages/MSBVAR/index.html) provides Bayesian estimation of vector autoregressive models. The [dlm](https://cloud.r-project.org/web/packages/dlm/index.html) package provides Bayesian and likelihood analysis of dynamic linear models (ie linear Gaussian state space models).
-   The [vars](https://cloud.r-project.org/web/packages/vars/index.html) package offer estimation, diagnostics, forecasting and error decomposition of VAR and SVAR model in a classical framework.
-   The [dyn](https://cloud.r-project.org/web/packages/dyn/index.html) and [dynlm](https://cloud.r-project.org/web/packages/dynlm/index.html) are suitable for dynamic (linear) regression models.
-   Several packages provide wavelet analysis functionality: [rwt](https://cloud.r-project.org/web/packages/rwt/index.html), [wavelets](https://cloud.r-project.org/web/packages/wavelets/index.html), [waveslim](https://cloud.r-project.org/web/packages/waveslim/index.html), [wavethresh](https://cloud.r-project.org/web/packages/wavethresh/index.html). Some methods from chaos theory are provided by the package [tseriesChaos](https://cloud.r-project.org/web/packages/tseriesChaos/index.html). [tsDyn](https://cloud.r-project.org/web/packages/tsDyn/index.html) adds time series analysis based on dynamical systems therory.
-   The [forecast](https://cloud.r-project.org/web/packages/forecast/index.html) package adds functions for forecasting problems.
-   The [tsfa](https://cloud.r-project.org/web/packages/tsfa/index.html) package provides functions for time series factor analysis.
-   The [stochvol](https://cloud.r-project.org/web/packages/stochvol/index.html) package implements Bayesian estimation of stochastic volatility using Markov Chain Monte Carlo.

**Finance**

-   The Rmetrics suite of packages comprises [fArma](https://cloud.r-project.org/web/packages/fArma/index.html), [fAsianOptions](https://cloud.r-project.org/web/packages/fAsianOptions/index.html), [fAssets](https://cloud.r-project.org/web/packages/fAssets/index.html), [fBasics](https://cloud.r-project.org/web/packages/fBasics/index.html), [fBonds](https://cloud.r-project.org/web/packages/fBonds/index.html), [timeDate](https://cloud.r-project.org/web/packages/timeDate/index.html) (formerly: fCalendar), [fCopulae](https://cloud.r-project.org/web/packages/fCopulae/index.html), [fExoticOptions](https://cloud.r-project.org/web/packages/fExoticOptions/index.html), [fExtremes](https://cloud.r-project.org/web/packages/fExtremes/index.html), [fGarch](https://cloud.r-project.org/web/packages/fGarch/index.html), [fImport](https://cloud.r-project.org/web/packages/fImport/index.html), [fNonlinear](https://cloud.r-project.org/web/packages/fNonlinear/index.html), [fOptions](https://cloud.r-project.org/web/packages/fOptions/index.html), [fPortfolio](https://cloud.r-project.org/web/packages/fPortfolio/index.html), [fRegression](https://cloud.r-project.org/web/packages/fRegression/index.html), [timeSeries](https://cloud.r-project.org/web/packages/timeSeries/index.html) (formerly: fSeries), [fTrading](https://cloud.r-project.org/web/packages/fTrading/index.html), [fUnitRoots](https://cloud.r-project.org/web/packages/fUnitRoots/index.html) and contains a very large number of relevant functions for different aspect of empirical and computational finance.
-   The [RQuantLib](https://cloud.r-project.org/web/packages/RQuantLib/index.html) package provides several option-pricing functions as well as some fixed-income functionality from the QuantLib project to R.
-   The [quantmod](https://cloud.r-project.org/web/packages/quantmod/index.html) package offers a number of functions for quantitative modelling in finance as well as data acqusition, plotting and other utilities.
-   The [portfolio](https://cloud.r-project.org/web/packages/portfolio/index.html) package contains classes for equity portfolio management; the [portfolioSim](https://cloud.r-project.org/web/packages/portfolioSim/index.html) builds a related simulation framework. The [backtest](https://cloud.r-project.org/web/packages/backtest/index.html) offers tools to explore portfolio-based hypotheses about financial instruments. The [stockPortfolio](https://cloud.r-project.org/web/packages/stockPortfolio/index.html) package provides functions for single index, constant correlation and multigroup models. The [pa](https://cloud.r-project.org/web/packages/pa/index.html) package offers performance attribution functionality for equity portfolios.
-   The [PerformanceAnalytics](https://cloud.r-project.org/web/packages/PerformanceAnalytics/index.html) package contains a large number of functions for portfolio performance calculations and risk management.
-   The [TTR](https://cloud.r-project.org/web/packages/TTR/index.html) contains functions to construct technical trading rules in R.
-   The [financial](https://cloud.r-project.org/web/packages/financial/index.html) package can compute present values, cash flows and other simple finance calculations.
-   The [sde](https://cloud.r-project.org/web/packages/sde/index.html) package provides simulation and inference functionality for stochastic differential equations.
-   The [termstrc](https://cloud.r-project.org/web/packages/termstrc/index.html) and [YieldCurve](https://cloud.r-project.org/web/packages/YieldCurve/index.html) packages contain methods for the estimation of zero-coupon yield curves and spread curves based the parametric Nelson and Siegel (1987) method with the Svensson (1994) extension. The former package adds the McCulloch (1975) cubic splines approach, the latter package adds the Diebold and Li approach. The [SmithWilsonYieldCurve](https://cloud.r-project.org/web/packages/SmithWilsonYieldCurve/index.html) construct the yield curve using the Smith-Wilson approach based on LIBOR and SWAP rates.
-   The [vrtest](https://cloud.r-project.org/web/packages/vrtest/index.html) package contains a number of variance ratio tests for the weak-form of the efficient markets hypothesis.
-   The [gmm](https://cloud.r-project.org/web/packages/gmm/index.html) package provides generalized method of moments (GMM) estimations function that are often used when estimating the parameters of the moment conditions implied by an asset pricing model.
-   The [tawny](https://cloud.r-project.org/web/packages/tawny/index.html) package contains estimator based on random matrix theory as well as shrinkage methods to remove sampling noise when estimating sample covariance matrices.
-   The [opefimor](https://cloud.r-project.org/web/packages/opefimor/index.html) package by contains material to accompany the Iacus (2011) book entitled "Option Pricing and Estimation of Financial Models in R".
-   The [maRketSim](https://cloud.r-project.org/web/packages/maRketSim/index.html) package provides a market simulator, initially designed around the bond market.
-   The [BurStFin](https://cloud.r-project.org/web/packages/BurStFin/index.html) and [BurStMisc](https://cloud.r-project.org/web/packages/BurStMisc/index.html) package has a collection of function for Finance including the estimation of covariance matrices.
-   The [AmericanCallOpt](https://cloud.r-project.org/web/packages/AmericanCallOpt/index.html) package contains a pricer for different American call options.
-   The [VarSwapPrice](https://cloud.r-project.org/web/packages/VarSwapPrice/index.html) package can price a variance swap via a portfolio of European options contracts.
-   The [FinAsym](https://cloud.r-project.org/web/packages/FinAsym/index.html) package implements the Lee and Ready (1991) and Easley and O'Hara (1987) tests for, respectively, trade direction, and probability of informed trading.
-   The [parma](https://cloud.r-project.org/web/packages/parma/index.html) package provides support for portfolio allocation and risk management applications.
-   The [GUIDE](https://cloud.r-project.org/web/packages/GUIDE/index.html) package provides a *GUI* for *DE* rivatives and contains numerous pricer examples as well as interactive 2d and 3d plots to study these pricing functions.
-   The [SharpeR](https://cloud.r-project.org/web/packages/SharpeR/index.html) package contains a collection of tools for analyzing significance of trading strategies, based on the Sharpe ratio and overfit of the same.
-   The [RND](https://cloud.r-project.org/web/packages/RND/index.html) package implements various functions to extract risk-neutral densities from option prices.
-   [LSMonteCarlo](https://cloud.r-project.org/web/packages/LSMonteCarlo/index.html) can price American Options via the Least Squares Monte Carlo method
-   The [BenfordTests](https://cloud.r-project.org/web/packages/BenfordTests/index.html) package provides seven statistical tests and support functions for determining if numerical data could conform to Benford's law.
-   The [OptHedging](https://cloud.r-project.org/web/packages/OptHedging/index.html) package values call and put option portfolio and implements an optimal hedging strategy.
-   The [markovchain](https://cloud.r-project.org/web/packages/markovchain/index.html) package provides functionality to easily handle and analyse discrete Markov chains.
-   The [ycinterextra](https://cloud.r-project.org/web/packages/ycinterextra/index.html) package models yield curve interpolation and extrapolation using via the Nelson-Siegel, Svensson, or Smith-Wilson models, as well as Hermite cubic splines.
-   The [tvm](https://cloud.r-project.org/web/packages/tvm/index.html) package models provides functions for time value of money such as cashflows and yield curves.
-   The [MarkowitzR](https://cloud.r-project.org/web/packages/MarkowitzR/index.html) package provides functions to test the statistical signicance of Markowitz portfolios.
-   The [egcm](https://cloud.r-project.org/web/packages/egcm/index.html) package implements the Engle-Granger two-stage cointegration modeling procedure with a particular focus on pairs trading.
-   The [pbo](https://cloud.r-project.org/web/packages/pbo/index.html) package models the probability of backtest overfitting, performance degradation, probability of loss, and the stochastic dominance when analysing trading strategies.
-   The [OptionPricing](https://cloud.r-project.org/web/packages/OptionPricing/index.html) package implements efficient Monte Carlo algorithms for the price and the sensitivities of Asian and European Options under Geometric Brownian Motion.
-   The [matchingMarkets](https://cloud.r-project.org/web/packages/matchingMarkets/index.html) package implements a structural estimator to correct for the bias arising from endogenous matching (e.g. group formation in microfinance or matching of firms and venture capitalists).
-   The [restimizeapi](https://cloud.r-project.org/web/packages/restimizeapi/index.html) package interfaces the API at www.estimize.com which provides crowd-sourced earnings estimates.
-   The [credule](https://cloud.r-project.org/web/packages/credule/index.html) package is another pricer for credit default swaps.
-   The [covmat](https://cloud.r-project.org/web/packages/covmat/index.html) package provides several different methods for computing covariance matrices.
-   The [obAnalytics](https://cloud.r-project.org/web/packages/obAnalytics/index.html) package analyses and visualizes information from events in limit order book data.
-   The [bootTimeInference](https://cloud.r-project.org/web/packages/bootTimeInference/index.html) package performs robust resampling tests for the difference in Sharpe ratios.
-   The [derivmkts](https://cloud.r-project.org/web/packages/derivmkts/index.html) package adds a set of pricing and expository functions useful in teaching derivatives markets..

**Risk management**

-   Several packages provide functionality for Extreme Value Theory models: [evd](https://cloud.r-project.org/web/packages/evd/index.html), [evdbayes](https://cloud.r-project.org/web/packages/evdbayes/index.html), [evir](https://cloud.r-project.org/web/packages/evir/index.html), [extRemes](https://cloud.r-project.org/web/packages/extRemes/index.html), [ismev](https://cloud.r-project.org/web/packages/ismev/index.html).
-   The packages [CreditMetrics](https://cloud.r-project.org/web/packages/CreditMetrics/index.html) and [crp.CSFP](https://cloud.r-project.org/web/packages/crp.CSFP/index.html) provide function for modelling credit risks.
-   The [mvtnorm](https://cloud.r-project.org/web/packages/mvtnorm/index.html) package provides code for multivariate Normal and t-distributions.
-   The Rmetrics packages [fPortfolio](https://cloud.r-project.org/web/packages/fPortfolio/index.html) and [fExtremes](https://cloud.r-project.org/web/packages/fExtremes/index.html) also contain a number of relevant functions.
-   The [copula](https://cloud.r-project.org/web/packages/copula/index.html) and [fgac](https://cloud.r-project.org/web/packages/fgac/index.html) packages cover multivariate dependency structures using copula methods.
-   The [actuar](https://cloud.r-project.org/web/packages/actuar/index.html) package provides an actuarial perspective to risk management.
-   The [ghyp](https://cloud.r-project.org/web/packages/ghyp/index.html) package provides generalized hyberbolic distribution functions as well as procedures for VaR, CVaR or target-return portfolio optimizations.
-   The [ChainLadder](https://cloud.r-project.org/web/packages/ChainLadder/index.html) package provides functions for modeling insurance claim reserves; and the [lifecontingencies](https://cloud.r-project.org/web/packages/lifecontingencies/index.html) package provides functions for financial and actuarial evaluations of life contingencies.
-   The [frmqa](https://cloud.r-project.org/web/packages/frmqa/index.html) package aims to collect functions for Financial Risk Management and Quantitative Analysis.
-   The [ESG](https://cloud.r-project.org/web/packages/ESG/index.html) package can be used to model for asset projection, a scenario-based simulation approach.
-   The [riskSimul](https://cloud.r-project.org/web/packages/riskSimul/index.html) package provides efficient simulation procedures to estimate tail loss probabilities and conditional excess for a stock portfolios where log-returns are assumed to follow a t-copula model with generalized hyperbolic or t marginals.
-   The [GCPM](https://cloud.r-project.org/web/packages/GCPM/index.html) package anlyzes the default risk of credit portfolio using both analytical and simulation approaches.
-   The [FatTailsR](https://cloud.r-project.org/web/packages/FatTailsR/index.html) package provides a family of four distributions tailored to distribution with symmetric and asymmetric fat tails.
-   The [PortRisk](https://cloud.r-project.org/web/packages/PortRisk/index.html) computes portfolio risk attribution.

**Books**

-   The [FinTS](https://cloud.r-project.org/web/packages/FinTS/index.html) package provides an R companion to Tsay (2005), *Analysis of Financial Time Series* , 2nd ed. Wiley, and includes data sets, functions and script files to work some of the examples.
-   The [NMOF](https://cloud.r-project.org/web/packages/NMOF/index.html) package provides functions, examples and data from *Numerical Methods in Finance* by Manfred Gilli, Dietmar Maringer and Enrico Schumann (2011), including the different optimization heuristics such as Differential Evolution, Genetic Algorithms, Particle Swarms, and Threshold Accepting.
-   The [FRAPO](https://cloud.r-project.org/web/packages/FRAPO/index.html) package provides data sets and code for the book *Financial Risk Modelling and Portfolio Optimization with R* by Bernhard Paff (2013).

**Data and date management**

-   The [its](https://cloud.r-project.org/web/packages/its/index.html), [zoo](https://cloud.r-project.org/web/packages/zoo/index.html) and [timeDate](https://cloud.r-project.org/web/packages/timeDate/index.html) (part of Rmetrics) packages provide support for irregularly-spaced time series. The [xts](https://cloud.r-project.org/web/packages/xts/index.html) package extends [zoo](https://cloud.r-project.org/web/packages/zoo/index.html) specifically for financial time series. See the [TimeSeries](https://cloud.r-project.org/web/views/TimeSeries.html) task view for more details.
-   [timeDate](https://cloud.r-project.org/web/packages/timeDate/index.html) also addresses calendar issues such as recurring holidays for a large number of financial centers, and provides code for high-frequency data sets.
-   The [fame](https://cloud.r-project.org/web/packages/fame/index.html) package can access Fame time series databases (but also requires a Fame backend). The [tis](https://cloud.r-project.org/web/packages/tis/index.html) package provides time indices and time-indexed series compatible with Fame frequencies.
-   The [TSdbi](https://cloud.r-project.org/web/packages/TSdbi/index.html) package provides a unifying interface for several time series data base backends, and its SQL implementations provide a database table design.
-   The [IBrokers](https://cloud.r-project.org/web/packages/IBrokers/index.html) package provides access to the Interactive Brokers API for data access (but requires an account to access the service).
-   The [data.table](https://cloud.r-project.org/web/packages/data.table/index.html) package provides very efficient and fast access to in-memory data sets such as asset prices.
-   The [TFX](https://cloud.r-project.org/web/packages/TFX/index.html) package provides an interface to the TrueFX (TM) service for free streaming real-time and historical tick-by-tick market data for interbank foreign exchange rates at the millisecond resolution.
-   The package [highfrequency](https://cloud.r-project.org/web/packages/highfrequency/index.html) contains functionality to manage, clean and match highfrequency trades and quotes data and enables users to calculate various liquidity measures, estimate and forecast volatility, and investigate microstructure noise and intraday periodicity.
-   The [Rbitcoin](https://cloud.r-project.org/web/packages/Rbitcoin/index.html) package offers access to Bitcoin exchange APIs (mtgox, bitstamp, btce, kraken) via public and private API calls and integration of data structures for all markets.
-   The [bizdays](https://cloud.r-project.org/web/packages/bizdays/index.html) package compute business days if provided a list of holidays.
-   The [TAQMNGR](https://cloud.r-project.org/web/packages/TAQMNGR/index.html) package manages tick-by-tick (equity) transaction data performing 'cleaning', 'aggregation' and 'import' where cleaning and aggregation are performed according to Brownlees and Gallo (2006).
-   The [Rblpapi](https://cloud.r-project.org/web/packages/Rblpapi/index.html) package offers efficient access to the Bloomberg API and allows `bdp`, `bdh`, and `bds` queries as well as data retrieval both in (regular time-)bars and ticks (albeit without subsecond resolution).
-   The [finreportr](https://cloud.r-project.org/web/packages/finreportr/index.html) package can download reports from the SEC Edgar database, and relies on, inter alia, the [XBRL](https://cloud.r-project.org/web/packages/XBRL/index.html) package for parsing these reports.

### CRAN packages:

-   [actuar](https://cloud.r-project.org/web/packages/actuar/index.html)
-   [AmericanCallOpt](https://cloud.r-project.org/web/packages/AmericanCallOpt/index.html)
-   [backtest](https://cloud.r-project.org/web/packages/backtest/index.html)
-   [bayesGARCH](https://cloud.r-project.org/web/packages/bayesGARCH/index.html)
-   [BenfordTests](https://cloud.r-project.org/web/packages/BenfordTests/index.html)
-   [betategarch](https://cloud.r-project.org/web/packages/betategarch/index.html)
-   [bizdays](https://cloud.r-project.org/web/packages/bizdays/index.html)
-   [bootTimeInference](https://cloud.r-project.org/web/packages/bootTimeInference/index.html)
-   [BurStFin](https://cloud.r-project.org/web/packages/BurStFin/index.html)
-   [BurStMisc](https://cloud.r-project.org/web/packages/BurStMisc/index.html)
-   [CADFtest](https://cloud.r-project.org/web/packages/CADFtest/index.html)
-   [car](https://cloud.r-project.org/web/packages/car/index.html)
-   [ccgarch](https://cloud.r-project.org/web/packages/ccgarch/index.html)
-   [ChainLadder](https://cloud.r-project.org/web/packages/ChainLadder/index.html)
-   [copula](https://cloud.r-project.org/web/packages/copula/index.html)
-   [covmat](https://cloud.r-project.org/web/packages/covmat/index.html)
-   [CreditMetrics](https://cloud.r-project.org/web/packages/CreditMetrics/index.html)
-   [credule](https://cloud.r-project.org/web/packages/credule/index.html)
-   [crp.CSFP](https://cloud.r-project.org/web/packages/crp.CSFP/index.html)
-   [data.table](https://cloud.r-project.org/web/packages/data.table/index.html)
-   [derivmkts](https://cloud.r-project.org/web/packages/derivmkts/index.html)
-   [dlm](https://cloud.r-project.org/web/packages/dlm/index.html)
-   [dse](https://cloud.r-project.org/web/packages/dse/index.html)
-   [dyn](https://cloud.r-project.org/web/packages/dyn/index.html)
-   [dynlm](https://cloud.r-project.org/web/packages/dynlm/index.html)
-   [egcm](https://cloud.r-project.org/web/packages/egcm/index.html)
-   [ESG](https://cloud.r-project.org/web/packages/ESG/index.html)
-   [evd](https://cloud.r-project.org/web/packages/evd/index.html)
-   [evdbayes](https://cloud.r-project.org/web/packages/evdbayes/index.html)
-   [evir](https://cloud.r-project.org/web/packages/evir/index.html)
-   [extRemes](https://cloud.r-project.org/web/packages/extRemes/index.html)
-   [fame](https://cloud.r-project.org/web/packages/fame/index.html)
-   [fArma](https://cloud.r-project.org/web/packages/fArma/index.html) (core)
-   [fAsianOptions](https://cloud.r-project.org/web/packages/fAsianOptions/index.html) (core)
-   [fAssets](https://cloud.r-project.org/web/packages/fAssets/index.html) (core)
-   [FatTailsR](https://cloud.r-project.org/web/packages/FatTailsR/index.html)
-   [fBasics](https://cloud.r-project.org/web/packages/fBasics/index.html) (core)
-   [fBonds](https://cloud.r-project.org/web/packages/fBonds/index.html) (core)
-   [fCopulae](https://cloud.r-project.org/web/packages/fCopulae/index.html) (core)
-   [fExoticOptions](https://cloud.r-project.org/web/packages/fExoticOptions/index.html) (core)
-   [fExtremes](https://cloud.r-project.org/web/packages/fExtremes/index.html) (core)
-   [fgac](https://cloud.r-project.org/web/packages/fgac/index.html)
-   [fGarch](https://cloud.r-project.org/web/packages/fGarch/index.html) (core)
-   [fImport](https://cloud.r-project.org/web/packages/fImport/index.html) (core)
-   [financial](https://cloud.r-project.org/web/packages/financial/index.html)
-   [FinAsym](https://cloud.r-project.org/web/packages/FinAsym/index.html)
-   [finreportr](https://cloud.r-project.org/web/packages/finreportr/index.html)
-   [FinTS](https://cloud.r-project.org/web/packages/FinTS/index.html)
-   [fMultivar](https://cloud.r-project.org/web/packages/fMultivar/index.html) (core)
-   [fNonlinear](https://cloud.r-project.org/web/packages/fNonlinear/index.html) (core)
-   [fOptions](https://cloud.r-project.org/web/packages/fOptions/index.html) (core)
-   [forecast](https://cloud.r-project.org/web/packages/forecast/index.html)
-   [fPortfolio](https://cloud.r-project.org/web/packages/fPortfolio/index.html) (core)
-   [fracdiff](https://cloud.r-project.org/web/packages/fracdiff/index.html)
-   [fractal](https://cloud.r-project.org/web/packages/fractal/index.html)
-   [FRAPO](https://cloud.r-project.org/web/packages/FRAPO/index.html)
-   [fRegression](https://cloud.r-project.org/web/packages/fRegression/index.html) (core)
-   [frmqa](https://cloud.r-project.org/web/packages/frmqa/index.html)
-   [fTrading](https://cloud.r-project.org/web/packages/fTrading/index.html) (core)
-   [fUnitRoots](https://cloud.r-project.org/web/packages/fUnitRoots/index.html) (core)
-   [GCPM](https://cloud.r-project.org/web/packages/GCPM/index.html)
-   [gets](https://cloud.r-project.org/web/packages/gets/index.html)
-   [GEVStableGarch](https://cloud.r-project.org/web/packages/GEVStableGarch/index.html)
-   [ghyp](https://cloud.r-project.org/web/packages/ghyp/index.html)
-   [gmm](https://cloud.r-project.org/web/packages/gmm/index.html)
-   [gogarch](https://cloud.r-project.org/web/packages/gogarch/index.html)
-   [GUIDE](https://cloud.r-project.org/web/packages/GUIDE/index.html)
-   [highfrequency](https://cloud.r-project.org/web/packages/highfrequency/index.html)
-   [IBrokers](https://cloud.r-project.org/web/packages/IBrokers/index.html)
-   [ismev](https://cloud.r-project.org/web/packages/ismev/index.html)
-   [its](https://cloud.r-project.org/web/packages/its/index.html)
-   [lgarch](https://cloud.r-project.org/web/packages/lgarch/index.html)
-   [lifecontingencies](https://cloud.r-project.org/web/packages/lifecontingencies/index.html)
-   [lmtest](https://cloud.r-project.org/web/packages/lmtest/index.html)
-   [longmemo](https://cloud.r-project.org/web/packages/longmemo/index.html)
-   [LSMonteCarlo](https://cloud.r-project.org/web/packages/LSMonteCarlo/index.html)
-   [maRketSim](https://cloud.r-project.org/web/packages/maRketSim/index.html)
-   [markovchain](https://cloud.r-project.org/web/packages/markovchain/index.html)
-   [MarkowitzR](https://cloud.r-project.org/web/packages/MarkowitzR/index.html)
-   [matchingMarkets](https://cloud.r-project.org/web/packages/matchingMarkets/index.html)
-   [MSBVAR](https://cloud.r-project.org/web/packages/MSBVAR/index.html)
-   [mvtnorm](https://cloud.r-project.org/web/packages/mvtnorm/index.html)
-   [nlme](https://cloud.r-project.org/web/packages/nlme/index.html)
-   [NMOF](https://cloud.r-project.org/web/packages/NMOF/index.html)
-   [obAnalytics](https://cloud.r-project.org/web/packages/obAnalytics/index.html)
-   [opefimor](https://cloud.r-project.org/web/packages/opefimor/index.html)
-   [OptHedging](https://cloud.r-project.org/web/packages/OptHedging/index.html)
-   [OptionPricing](https://cloud.r-project.org/web/packages/OptionPricing/index.html)
-   [pa](https://cloud.r-project.org/web/packages/pa/index.html)
-   [parma](https://cloud.r-project.org/web/packages/parma/index.html)
-   [pbo](https://cloud.r-project.org/web/packages/pbo/index.html)
-   [PerformanceAnalytics](https://cloud.r-project.org/web/packages/PerformanceAnalytics/index.html) (core)
-   [portfolio](https://cloud.r-project.org/web/packages/portfolio/index.html)
-   [portfolioSim](https://cloud.r-project.org/web/packages/portfolioSim/index.html)
-   [PortRisk](https://cloud.r-project.org/web/packages/PortRisk/index.html)
-   [quantmod](https://cloud.r-project.org/web/packages/quantmod/index.html)
-   [Rbitcoin](https://cloud.r-project.org/web/packages/Rbitcoin/index.html)
-   [Rblpapi](https://cloud.r-project.org/web/packages/Rblpapi/index.html)
-   [Rcmdr](https://cloud.r-project.org/web/packages/Rcmdr/index.html)
-   [restimizeapi](https://cloud.r-project.org/web/packages/restimizeapi/index.html)
-   [riskSimul](https://cloud.r-project.org/web/packages/riskSimul/index.html)
-   [rmgarch](https://cloud.r-project.org/web/packages/rmgarch/index.html)
-   [RND](https://cloud.r-project.org/web/packages/RND/index.html)
-   [RQuantLib](https://cloud.r-project.org/web/packages/RQuantLib/index.html)
-   [rugarch](https://cloud.r-project.org/web/packages/rugarch/index.html)
-   [rwt](https://cloud.r-project.org/web/packages/rwt/index.html)
-   [sandwich](https://cloud.r-project.org/web/packages/sandwich/index.html)
-   [sde](https://cloud.r-project.org/web/packages/sde/index.html)
-   [SharpeR](https://cloud.r-project.org/web/packages/SharpeR/index.html)
-   [SmithWilsonYieldCurve](https://cloud.r-project.org/web/packages/SmithWilsonYieldCurve/index.html)
-   [stochvol](https://cloud.r-project.org/web/packages/stochvol/index.html)
-   [stockPortfolio](https://cloud.r-project.org/web/packages/stockPortfolio/index.html)
-   [strucchange](https://cloud.r-project.org/web/packages/strucchange/index.html)
-   [TAQMNGR](https://cloud.r-project.org/web/packages/TAQMNGR/index.html)
-   [tawny](https://cloud.r-project.org/web/packages/tawny/index.html)
-   [termstrc](https://cloud.r-project.org/web/packages/termstrc/index.html)
-   [TFX](https://cloud.r-project.org/web/packages/TFX/index.html)
-   [timeDate](https://cloud.r-project.org/web/packages/timeDate/index.html) (core)
-   [timeSeries](https://cloud.r-project.org/web/packages/timeSeries/index.html) (core)
-   [timsac](https://cloud.r-project.org/web/packages/timsac/index.html)
-   [tis](https://cloud.r-project.org/web/packages/tis/index.html)
-   [TSdbi](https://cloud.r-project.org/web/packages/TSdbi/index.html)
-   [tsDyn](https://cloud.r-project.org/web/packages/tsDyn/index.html)
-   [tseries](https://cloud.r-project.org/web/packages/tseries/index.html) (core)
-   [tseriesChaos](https://cloud.r-project.org/web/packages/tseriesChaos/index.html)
-   [tsfa](https://cloud.r-project.org/web/packages/tsfa/index.html)
-   [TTR](https://cloud.r-project.org/web/packages/TTR/index.html)
-   [tvm](https://cloud.r-project.org/web/packages/tvm/index.html)
-   [urca](https://cloud.r-project.org/web/packages/urca/index.html) (core)
-   [vars](https://cloud.r-project.org/web/packages/vars/index.html)
-   [VarSwapPrice](https://cloud.r-project.org/web/packages/VarSwapPrice/index.html)
-   [vrtest](https://cloud.r-project.org/web/packages/vrtest/index.html)
-   [wavelets](https://cloud.r-project.org/web/packages/wavelets/index.html)
-   [waveslim](https://cloud.r-project.org/web/packages/waveslim/index.html)
-   [wavethresh](https://cloud.r-project.org/web/packages/wavethresh/index.html)
-   [XBRL](https://cloud.r-project.org/web/packages/XBRL/index.html)
-   [xts](https://cloud.r-project.org/web/packages/xts/index.html) (core)
-   [ycinterextra](https://cloud.r-project.org/web/packages/ycinterextra/index.html)
-   [YieldCurve](https://cloud.r-project.org/web/packages/YieldCurve/index.html)
-   [Zelig](https://cloud.r-project.org/web/packages/Zelig/index.html)
-   [zoo](https://cloud.r-project.org/web/packages/zoo/index.html) (core)

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
