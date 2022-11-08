
## CRAN Task View Empirical Finance

Maintainer: [Dirk Eddelbuettel](https://dirk.eddelbuettel.com)  
Date: 2022-11-08


This CRAN Task View contains a list of packages useful for empirical work in Finance, grouped by
topic.

Besides these packages, a very wide variety of functions suitable for empirical work in Finance is
provided by both the basic R system (and its set of recommended core packages), and a number of
other packages on the [Comprehensive R Archive Network
(CRAN)](https://cran.r-project.org). Consequently, several of the other CRAN Task Views may contain
suitable packages, in particular the `r view("Econometrics")`, `r view("Optimization")`,
`r view("Robust")`, and `r view("TimeSeries")` Task Views.

The `ctv` package supports these Task Views. Its functions `install.views` and `update.views` allow,
respectively, installation or update of packages from a given Task View; the option `coreOnly` can
restrict operations to packages labeled as *core* below.

Contributions are always welcome and encouraged, either via [e-mail to the
maintainer](mailto:dirk.eddelbuettel@r-project.org) or by submitting an issue or pull request in the
GitHub repository linked above. See the [Contributing
page](https://github.com/cran-task-views/ctv/blob/main/Contributing.md) in the [CRAN Task
Views](https://github.com/cran-task-views) repo for details.

### Standard regression models

-   A detailed overview of the available regression methodologies is provided by the
    `r view("Econometrics")` task view. This is complemented by the `r view("Robust")` task view, which
    focuses on more robust and resistant methods.
-   Linear models such as ordinary least squares (OLS) can be estimated by `lm()` (from by the stats
    package contained in the basic R distribution). Maximum Likelihood (ML) estimation can be
    undertaken with the standard `optim()` function. Many other suitable methods are listed in the
    `r view("Optimization")` view.  Non-linear least squares can be estimated with the `nls()`
    function, as well as with `nlme()` from the `r pkg("nlme")` package.
-   For the linear model, a variety of regression diagnostic tests are provided by the `r pkg("car")`,
    `r pkg("lmtest")`, `r pkg("strucchange")`, `r pkg("urca", priority = "core")`, and
    `r pkg("sandwich")` packages. The `r pkg("Rcmdr")` package provide user interfaces that may be
    of interest as well.

### Time series

-   A detailed overview of tools for time series analysis can be found in the `r view("TimeSeries")`
    task view. Below a brief overview of the most important methods in finance is given.
-   Classical time series functionality is provided by the `arima()` and `KalmanLike()` commands in
    the basic R distribution.
-   The `r pkg("dse")` and `r pkg("timsac")` packages provide a variety of more advanced estimation
    methods; `r pkg("fracdiff")` can estimate fractionally integrated series; `r pkg("longmemo")`
    covers related material.
-   For volatility modeling, the standard GARCH(1,1) model can be estimated with the `garch()`
    function in the `r pkg("tseries", priority = "core")` package. Rmetrics (see below) contains the
    `r pkg("fGarch", priority = "core")` package which has additional models. The `r pkg("rugarch",
    priority = "core")` package can be used to model a variety of univariate GARCH models with
    extensions such as ARFIMA, in-mean, external regressors and various other specifications; with
    methods for fit, forecast, simulation, inference and plotting are provided too. The
    `r pkg("rmgarch")` builds on it to provide the ability to estimate several multivariate GARCH
    models. The `r pkg("betategarch")` package can estimate and simulate the Beta-t-EGARCH model by
    Harvey. The `r pkg("bayesGARCH")` package can perform Bayesian estimation of a GARCH(1,1) model
    with Student's t innovations. For multivariate models, the `r pkg("gogarch")` package provides
    functions for generalized orthogonal GARCH models. The `r pkg("gets")` package (which was
    preceded by a related package AutoSEARCH) provides automated general-to-specific model selection
    of the mean and log-volatility of a log-ARCH-X model. The `r pkg("lgarch")` package can estimate
    and fit log-GARCH models. The `r pkg("garchx")` package estimate GARCH models with leverage and
    external covariates. The `r pkg("bmgarch")` package fits several multivariate GARCH models in a
    Bayesian setting. 
-   Unit root and cointegration tests are provided by `r pkg("tseries")`, and `r pkg("urca")`. The
    Rmetrics packages `r pkg("timeSeries", priority = "core")` and `r pkg("fMultivar", priority =
    "core")` contain a number of estimation functions for ARMA, GARCH, long memory models, unit
    roots and more. The `r pkg("CADFtest")` package implements the Hansen unit root test.
<!-- -   `r pkg("dlm")` package provides Bayesian and likelihood analysis of dynamic linear models -->
<!--     (i.e. linear Gaussian state space models). -->
-   The `r pkg("vars")` package offer estimation, diagnostics, forecasting and error decomposition
    of VAR and SVAR model in a classical framework.
-   The `r pkg("dyn")` and `r pkg("dynlm")` packages are suitable for dynamic (linear) regression
    models.
-   Several packages provide wavelet analysis functionality: `r pkg("wavelets")`,
    `r pkg("waveslim")`, `r pkg("wavethresh")`.  Some methods from chaos theory are provided by the
    package `r pkg("tseriesChaos")`. `r pkg("tsDyn")` adds time series analysis based on dynamical
    systems theory.
-   The `r pkg("forecast")` package adds functions for forecasting problems.
-   The `r pkg("stochvol")` package implements Bayesian estimation of stochastic volatility using
    Markov Chain Monte Carlo, and `r pkg("factorstochvol")` extends this to the multivariate case.
-   The `r pkg("MSGARCH")` package adds methods to fit (by Maximum Likelihood or Bayesian),
    simulate, and forecast various Markov-Switching GARCH processes.
-   The `r pkg("DriftBurstHypothesis")` package estimates a t-test statistics for the explosive
    drift burst hypothesis (Christensen, Oomen and Reno, 2018).
-   Package `r pkg("lmForc")` various in-sample, out-of-sample, pseudo-out-of-sample and benchmark
    linear model forecast tests.

### Finance

-   The Rmetrics suite of packages comprises 
    `r pkg("fAssets", priority = "core")`,
    `r pkg("fBasics", priority = "core")`, 
    `r pkg("fBonds", priority = "core")`, 
    `r pkg("timeDate", priority = "core")` (formerly: fCalendar), 
    `r pkg("fCopulae", priority = "core")`,
    `r pkg("fExtremes", priority = "core")`, 
    `r pkg("fGarch")`, 
    `r pkg("fImport", priority = "core")`, 
    `r pkg("fNonlinear", priority = "core")`,
    `r pkg("fPortfolio", priority = "core")`,
    `r pkg("fRegression", priority = "core")`, 
    `r pkg("timeSeries")` (formerly: fSeries),
    `r pkg("fTrading", priority = "core")`, and contains a very large number of relevant functions for
    different aspect of empirical and computational finance.
-   The `r pkg("RQuantLib")` package provides several option-pricing functions as well as some
    fixed-income functionality from the QuantLib project to R. The `r pkg("RcppQuantuccia")`
    provides a smaller subset of QuantLib functionality as a header-only library; at current only
    some calendaring functionality is exposed.
-   The `r pkg("quantmod")` package offers a number of functions for quantitative modelling in
    finance as well as data acquisition, plotting and other utilities.
-   The `r pkg("backtest")` offers tools to explore portfolio-based hypotheses about financial
    instruments. The `r pkg("pa")` package offers performance attribution functionality for equity
    portfolios.
-   The `r pkg("PerformanceAnalytics", priority = "core")` package contains a large number of
    functions for portfolio performance calculations and risk management.
-   The `r pkg("TTR")` contains functions to construct technical trading rules in R.
-   The `r pkg("sde")` package provides simulation and inference functionality for stochastic
    differential equations.
-   The `r pkg("vrtest")` package contains a number of variance ratio tests for the weak-form of the
    efficient markets hypothesis.
-   The `r pkg("gmm")` package provides generalized method of moments (GMM) estimations function
    that are often used when estimating the parameters of the moment conditions implied by an asset
    pricing model.
-   The `r pkg("BurStFin")` and `r pkg("BurStMisc")` package has a collection of function for
    Finance including the estimation of covariance matrices.
-   The `r pkg("AmericanCallOpt")` package contains a pricer for different American call options.
-   The `r pkg("FinAsym")` package implements the Lee and Ready (1991) and Easley and O'Hara (1987)
    tests for, respectively, trade direction, and probability of informed trading.
-   The `r pkg("parma")` package provides support for portfolio allocation and risk management
    applications.
-   The `r pkg("GUIDE")` package provides a *GUI* for *DE* rivatives and contains numerous pricer
    examples as well as interactive 2d and 3d plots to study these pricing functions.
-   The `r pkg("SharpeR")` package contains a collection of tools for analyzing significance of
    trading strategies, based on the Sharpe ratio and overfit of the same.
-   The `r pkg("RND")` package implements various functions to extract risk-neutral densities from
    option prices.
-   The `r pkg("LSMonteCarlo")` package can price American Options via the Least Squares Monte Carlo
    method.
-   The `r pkg("BenfordTests")` package provides seven statistical tests and support functions for
    determining if numerical data could conform to Benford's law.
-   The `r pkg("OptHedging")` package values call and put option portfolio and implements an optimal
    hedging strategy.
-   The `r pkg("markovchain")` package provides functionality to easily handle and analyse discrete
    Markov chains.
-   The `r pkg("tvm")` package models provides functions for time value of money such as cashflows
    and yield curves.
-   The `r pkg("MarkowitzR")` package provides functions to test the statistical significance of
    Markowitz portfolios.
-   The `r pkg("pbo")` package models the probability of backtest overfitting, performance
    degradation, probability of loss, and the stochastic dominance when analysing trading
    strategies.
-   The `r pkg("OptionPricing")` package implements efficient Monte Carlo algorithms for the price
    and the sensitivities of Asian and European Options under Geometric Brownian Motion.
-   The `r pkg("matchingMarkets")` package implements a structural estimator to correct for the bias
    arising from endogenous matching (e.g. group formation in microfinance or matching of firms and
    venture capitalists).
-   The `r pkg("restimizeapi")` package interfaces the API at www.estimize.com which provides
    crowd-sourced earnings estimates.
-   The `r pkg("credule")` package is another pricer for credit default swaps.
-   The `r pkg("obAnalytics")` package analyses and visualizes information from events in limit
    order book data.
-   The `r pkg("derivmkts")` package adds a set of pricing and expository functions useful in
    teaching derivatives markets.
-   The `r pkg("PortfolioEffectHFT")` package provides portfolio analysis suitable for intra-day and
    high-frequency data, and also interfaces the PortfolioEffect service.
-   The `r pkg("ragtop")` package prices equity derivatives under an extension to Black and Scholes
    supporting default under a power-law link price and hazard rate.
-   The `r pkg("InfoTrad")` packages estimates PIN and extends it to different factorization and
    estimation algorithms.
-   The `r pkg("FinancialMath")` package contains financial math and derivatives pricing functions
    as required by the actuarial exams by the Society of Actuaries and Casualty Actuarial Society
    'Financial Mathematics' exam.
-   The `r pkg("tidyquant")` package re-arranges functionality from several other key packages for
    use in the so-called tidyverse.
-   The `r pkg("BCC1997")` prices European options under the Bakshi, Cao anc Chen (1997) model for
    stochastic volatility, stochastic rates and random jumps.
-   The `r pkg("Sim.DiffProc")` package provides functions to simulate and analyse multidimensional
    Itô and Stratonovitch stochastic calculus for continuous-time models.
-   The `r pkg("BLModel")` package computes the posterior distribution in a Black-Litterman model
    from a prior distribution given by asset returns and continuous distribution of views given by
    an external function.
<!-- -   The `r pkg("rpatrec")` package aims to recognise charting patterns in (financial) time series -->
<!--     data. -->
-   The `r pkg("PortfolioOptim")` can solve both small and large sample portfolio optimization.
<!-- -   The `r pkg("estudy2")` package implements most commonly used parametric and nonparametric -->
<!--     event-study methodology tests. -->
-   The `r pkg("DtD")` package computes the *distance to default* per Merton's model.
-   The `r pkg("PeerPerformance")` package analyzes performance of investments funds relative to its
    peers in a pairwise manner that is robust to false discoveries.
-   The `r pkg("crseEventStudy")` package provides another event-study tool to analyse abnormal
    return in long-horizon events.
-   The `r pkg("simfinapi")` package provides R access to [SimFin](https://SimFin.com) fundamental
    financial statement data (given an API key).
-   The `r pkg("NFCP")` package models commodity prices via an n-factor term structure estimation.
-   The `r pkg("LSMRealOptions")` package uses least-squares Monte Carlo to value American and Real
    options.
-   The `r pkg("AssetCorr")` package estimates intra- and inter-cohort correlations from default
    data in a Vasicek credit portfolio model.
-   The `r pkg("ichimoku")` package provides tools for creating and visualising Ichimoku Kinko Hyo
    strategies, and provides an interface to the OANDA fxTrade API for retrieving historical and
    live streaming price data (which requires free registration).
-   The `r pkg("greeks")` package calculate sensitivities of financial option prices for European
    and Asian and American options in the Black Scholes model.
-   The `r pkg("RTL")` (Risk Tool Library) package offers a collection of functions and metadata to
    complement core packages in finance and commodities, including futures expiry tables.
-   The `r pkg("GARCHSK")` package estimates GARCHSK and GJRSK models allowing for time-varying
    volatility, skewness and kurtosis.
-   The `r pkg("bidask")` package offers a novel procedure to estimate bid-ask spreads from OHLC
    data, and implements other reference models.
-   The `r pkg("strand")` package adds a framework for discrete (share-level) simulations of
    investment strategies.
-   The `r pkg("HDShOP")` package constructs shrinkage estimators of high-dimensional mean-variance
    portfolios and performs high-dimensional tests on optimality, and the `r pkg("DOSPortfolio")`
    package uses it to constructs dynamic optimal shrinkage estimators for the weights of the global
    minimum variance portfolio.
-   The `r pkg("fixedincome")` package adds functions for fixed-income models, calculation, models and curves.

### Risk management

-   The packages `r pkg("qrmtools")` and `r pkg("qrmdata")` provide tools and data for standard
    tasks in Quantitative Risk Management (QRM) and accompany the book of [McNeil, Frey, Embrechts
    (2005, 2015, "Quantitative Risk Management: Concepts, Techniques,
    Tools")](https://press.princeton.edu/books/hardcover/9780691166278/quantitative-risk-management).
-   The Task View `r view("ExtremeValue")` regroups a number of relevant packages.
-   The `r pkg("mvtnorm")` package provides code for multivariate Normal and t-distributions.
-   The package `r pkg("nvmix")` provides functionality for multivariate normal variance mixtures
    (including normal and t for non-integer degrees of freedom).
-   The Rmetrics packages `r pkg("fPortfolio")` and `r pkg("fExtremes")` also contain a number of
    relevant functions.
-   The packages `r pkg("copula")` and `r pkg("copulaData")` cover a wide range of modeling tasks
    for copulas.
-   The `r pkg("actuar")` package provides an actuarial perspective to risk management.
-   The `r pkg("ghyp")` package provides generalized hyberbolic distribution functions as well as
    procedures for VaR, CVaR or target-return portfolio optimizations.
-   The `r pkg("ChainLadder")` package provides functions for modeling insurance claim reserves; and
    the `r pkg("lifecontingencies")` package provides functions for financial and actuarial
    evaluations of life contingencies.
-   The `r pkg("ESG")` package can be used to model for asset projection, a scenario-based
    simulation approach.
-   The `r pkg("riskSimul")` package provides efficient simulation procedures to estimate tail loss
    probabilities and conditional excess for a stock portfolios where log-returns are assumed to
    follow a t-copula model with generalized hyperbolic or t marginals.
-   The `r pkg("GCPM")` package analyzes the default risk of credit portfolio using both analytical
    and simulation approaches.
-   The `r pkg("FatTailsR")` package provides a family of four distributions tailored to
    distribution with symmetric and asymmetric fat tails.
-   The `r pkg("Dowd")` package contains functions ported from the 'MMR2' toolbox offered in Kevin
    Dowd's book "Measuring Market Risk".
-   The `r pkg("PortRisk")` package computes portfolio risk attribution.
-   The `r pkg("NetworkRiskMeasures")` package implements some risk measures for financial networks
    such as DebtRank, Impact Susceptibility, Impact Diffusion and Impact Fluidity.
-   The `r pkg("Risk")` package computes 26 financial risk measures for any continuous distribution.
-   The `r pkg("RiskPortfolios")` package constructs risk-based portfolios as per the corresponding
    papers by Ardia et al.
-   The `r pkg("reinsureR")` package models reinsurances a class Claims whose objective is to store
    claims and premiums, on which different treaties can be applied.
-   The `r pkg("RM2006")` package estimates conditional covariance matrix using the RiskMetrics 2006
    methodology described in Zumbach (2007).
-   The `r pkg("cvar")` package computes expected shortfall and value at risk for continuous
    distributions.
-   `r pkg("riskParityPortfolio")` offers fast implementations for constructing risk-parity
    portfolios.
-   The `r pkg("monobin")` package performs monotonic binning of numeric risk factor in credit
    rating models (PD, LGD, EAD) development.
-   The `r pkg("etrm")` package contains a collection of functions to perform core tasks within
    energy trading and risk management (ETRM).
-   Package `r pkg("ufRisk")` offers multiple Value at Risk and Expected Shortfall measures from both
    parametric and semiparametrics models.
-   Packages `r pkg("bondAnalyst")` and `r pkg("stockAnalyst")` provide a number of, respectively,
    bond pricing  and fixed-income valuation functions and fundamental equity valuation function
    corresponding to standard  industry practices for risk and return. 
-   Packages `r pkg("bearishTrader")`,  `r pkg("bullishTrader")`, and `r pkg("volatilityTrader")`
    support trading strategies and analysis for, respectively, directional views or volatility regimes.

### Books

-   The `r pkg("NMOF")` package provides functions, examples and data from *Numerical Methods and
    Optimization in Finance* by Manfred Gilli, Dietmar Maringer and Enrico Schumann (2011),
    including the different optimization heuristics such as Differential Evolution, Genetic
    Algorithms, Particle Swarms, and Threshold Accepting.
-   The `r pkg("FRAPO")` package provides data sets and code for the book *Financial Risk Modelling
    and Portfolio Optimization with R* by Bernhard Pfaff (2013).

### Data and date management

-   The `r pkg("zoo", priority = "core")` and `r pkg("timeDate")` (part of Rmetrics) packages
    provide support for irregularly-spaced time series. The `r pkg("xts", priority = "core")`
    package extends `r pkg("zoo")` specifically for financial time series.  See the
    `r view("TimeSeries")` task view for more details.
-   `r pkg("timeDate")` also addresses calendar issues such as recurring holidays for a large number
    of financial centers, and provides code for high-frequency data sets.
-   The `r pkg("fame")` package can access Fame time series databases (but also requires a Fame
    backend). The `r pkg("tis")` package provides time indices and time-indexed series compatible
    with Fame frequencies.
<!-- -   The `r pkg("TSdbi")` package provides a unifying interface for several time series data base -->
<!--     backends, and its SQL implementations provide a database table design. -->
-   The `r pkg("IBrokers")` package provides access to the Interactive Brokers API for data access
    (but requires an account to access the service).
-   The `r pkg("data.table")` package provides very efficient and fast access to in-memory data sets
    such as asset prices.
-   The package `r pkg("highfrequency")` contains functionality to manage, clean and match
    highfrequency trades and quotes data and enables users to calculate various liquidity measures,
    estimate and forecast volatility, and investigate microstructure noise and intraday periodicity.
-   The `r pkg("bizdays")` package compute business days if provided a list of holidays.
-   The `r pkg("TAQMNGR")` package manages tick-by-tick (equity) transaction data performing
    'cleaning', 'aggregation' and 'import' where cleaning and aggregation are performed according to
    Brownlees and Gallo (2006).
-   The `r pkg("Rblpapi")` package offers efficient access to the Bloomberg API and allows `bdp`,
    `bdh`, and `bds` queries as well as data retrieval both in (regular time-)bars and ticks (albeit
    without subsecond resolution).
-   The `r pkg("finreportr")` package can download reports from the SEC Edgar database, and relies
    on, inter alia, the `r pkg("XBRL")` package for parsing these reports.
-   The `r pkg("GetTDData")` package imports Brazilian government bonds data (such as LTN, NTN-B and
    LFT ) from the Tesouro Direto website.
-   The `r pkg("fmdates")` package implements common date calculations according to the ISDA
    schedules, and can check for business in different locales.
-   Data from Kenneth French's website can be downloaded with packages `r pkg("FFdownload")` and
    `r pkg("frenchdata")`. Individual datasets can also be downloaded with function `French` in package
    `r pkg("NMOF")`.



### Links
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
-   [Textbook "Tidy Finance with R" with many empirical finance applications](http://www.tidy-finance.org//)
