
**Please note that new home of this _CRAN Task View: Empirical Finance_ in in [this repo](https://github.com/cran-task-views/Finance) in the [cran-task-views organization](https://github.com/cran-task-views).**  This repository served for an earlier stage in the evolution of the Task Views and will remain to preserve links and attributions, but will likely not be extended.

## CRAN Task View: Empirical Finance


**Maintainer:** Dirk Eddelbuettel                           
**Contact:**    Dirk.Eddelbuettel at R-project.org          
**Version:**    2021-09-24                                  
**URL:**        <https://CRAN.R-project.org/view=Finance>   

<div>

This CRAN Task View contains a list of packages useful for empirical
work in Finance, grouped by topic.

Besides these packages, a very wide variety of functions suitable for
empirical work in Finance is provided by both the basic R system (and
its set of recommended core packages), and a number of other packages on
the Comprehensive R Archive Network (CRAN). Consequently, several of the
other CRAN Task Views may contain suitable packages, in particular the
[Econometrics](https://cran.r-project.org/web/views/Econometrics.html),
[Multivariate](https://cran.r-project.org/web/views/Multivariate.html),
[Optimization](https://cran.r-project.org/web/views/Optimization.html),
[Robust](https://cran.r-project.org/web/views/Robust.html),
[SocialSciences](https://cran.r-project.org/web/views/SocialSciences.html)
and [TimeSeries](https://cran.r-project.org/web/views/TimeSeries.html)
Task Views.

The ctv package supports these Task Views. Its functions install.views
and update.views allow, respectively, installation or update of packages
from a given Task View; the option coreOnly can restrict operations to
packages labeled as *core* below.

Contributions are always welcome, and encouraged. Since the start of
this CRAN task view in April 2005, most contributions have arrived as
email suggestions. The source file for this particular task view file
now also reside in a GitHub repository (see below) so that pull requests
are also possible.

**Standard regression models**

-   A detailed overview of the available regression methodologies is
    provided by the
    [Econometrics](https://cran.r-project.org/web/views/Econometrics.html)
    task view. This is complemented by the
    [Robust](https://cran.r-project.org/web/views/Robust.html) task
    view, which focuses on more robust and resistant methods.
-   Linear models such as ordinary least squares (OLS) can be estimated
    by lm() (from by the stats package contained in the basic R
    distribution). Maximum Likelihood (ML) estimation can be undertaken
    with the standard optim() function. Many other suitable methods are
    listed in the
    [Optimization](https://cran.r-project.org/web/views/Optimization.html)
    view. Non-linear least squares can be estimated with the nls()
    function, as well as with nlme() from the
    [nlme](https://cran.r-project.org/package=nlme) package.
-   For the linear model, a variety of regression diagnostic tests are
    provided by the [car](https://cran.r-project.org/package=car),
    [lmtest](https://cran.r-project.org/package=lmtest),
    [strucchange](https://cran.r-project.org/package=strucchange),
    [urca](https://cran.r-project.org/package=urca), and
    [sandwich](https://cran.r-project.org/package=sandwich) packages. The
    [Rcmdr](https://cran.r-project.org/package=Rcmdr) package provide user
    interfaces that may be of interest as well.

**Time series**

-   A detailed overview of tools for time series analysis can be found
    in the
    [TimeSeries](https://cran.r-project.org/web/views/TimeSeries.html)
    task view. Below a brief overview of the most important methods in
    finance is given.
-   Classical time series functionality is provided by the arima() and
    KalmanLike() commands in the basic R distribution.
-   The [dse](https://cran.r-project.org/package=dse) and
    [timsac](https://cran.r-project.org/package=timsac) packages provide a variety
    of more advanced estimation methods;
    [fracdiff](https://cran.r-project.org/package=fracdiff) can estimate
    fractionally integrated series;
    [longmemo](https://cran.r-project.org/package=longmemo) covers related material.
-   For volatility modeling, the standard GARCH(1,1) model can be
    estimated with the garch() function in the
    [tseries](https://cran.r-project.org/package=tseries) package. Rmetrics (see
    below) contains the [fGarch](https://cran.r-project.org/package=fGarch) package
    which has additional models. The
    [rugarch](https://cran.r-project.org/package=rugarch) package can be used to
    model a variety of univariate GARCH models with extensions such as
    ARFIMA, in-mean, external regressors and various other
    specifications; with methods for fit, forecast, simulation,
    inference and plotting are provided too. The
    [rmgarch](https://cran.r-project.org/package=rmgarch) builds on it to provide
    the ability to estimate several multivariate GARCH models. The
    [betategarch](https://cran.r-project.org/package=betategarch) package can
    estimate and simulate the Beta-t-EGARCH model by Harvey. The
    [bayesGARCH](https://cran.r-project.org/package=bayesGARCH) package can perform
    Bayesian estimation of a GARCH(1,1) model with Student's t
    innovations. For multivariate models, the
    [gogarch](https://cran.r-project.org/package=gogarch) package provides functions
    for generalized orthogonal GARCH models. The
    [gets](https://cran.r-project.org/package=gets) package (which was preceded by a
    related package AutoSEARCH) provides automated general-to-specific
    model selection of the mean and log-volatility of a log-ARCH-X
    model. The [lgarch](https://cran.r-project.org/package=lgarch) package can
    estimate and fit log-GARCH models. The
    [garchx](https://cran.r-project.org/package=garchx) package estimate GARCH
    models with leverage and external covariates. The
    [bmgarch](https://cran.r-project.org/package=bmgarch) package fits several
    multivariate GARCH models in a Bayesian setting. The
    [garchmodels](https://cran.r-project.org/package=garchmodels) package wraps the
    [rugarch](https://cran.r-project.org/package=rugarch) and
    [rmgarch](https://cran.r-project.org/package=rmgarch) packages.
-   Unit root and cointegration tests are provided by
    [tseries](https://cran.r-project.org/package=tseries), and
    [urca](https://cran.r-project.org/package=urca). The Rmetrics packages
    [timeSeries](https://cran.r-project.org/package=timeSeries) and
    [fMultivar](https://cran.r-project.org/package=fMultivar) contain a number of
    estimation functions for ARMA, GARCH, long memory models, unit roots
    and more. The [CADFtest](https://cran.r-project.org/package=CADFtest) package
    implements the Hansen unit root test.
-   [dlm](https://cran.r-project.org/package=dlm) package provides Bayesian and
    likelihood analysis of dynamic linear models (i.e. linear Gaussian
    state space models).
-   The [vars](https://cran.r-project.org/package=vars) package offer estimation,
    diagnostics, forecasting and error decomposition of VAR and SVAR
    model in a classical framework.
-   The [dyn](https://cran.r-project.org/package=dyn) and
    [dynlm](https://cran.r-project.org/package=dynlm) packages are suitable for
    dynamic (linear) regression models.
-   Several packages provide wavelet analysis functionality:
    [rwt](https://cran.r-project.org/package=rwt),
    [wavelets](https://cran.r-project.org/package=wavelets),
    [waveslim](https://cran.r-project.org/package=waveslim),
    [wavethresh](https://cran.r-project.org/package=wavethresh). Some methods from
    chaos theory are provided by the package
    [tseriesChaos](https://cran.r-project.org/package=tseriesChaos).
    [tsDyn](https://cran.r-project.org/package=tsDyn) adds time series analysis
    based on dynamical systems theory.
-   The [forecast](https://cran.r-project.org/package=forecast) package adds
    functions for forecasting problems.
-   The [stochvol](https://cran.r-project.org/package=stochvol) package implements
    Bayesian estimation of stochastic volatility using Markov Chain
    Monte Carlo, and
    [factorstochvol](https://cran.r-project.org/package=factorstochvol) extends this
    to the multivariate case.
-   The [MSGARCH](https://cran.r-project.org/package=MSGARCH) package adds methods
    to fit (by Maximum Likelihood or Bayesian), simulate, and forecast
    various Markov-Switching GARCH processes.
-   The
    [DriftBurstHypothesis](https://cran.r-project.org/package=DriftBurstHypothesis)
    package estimates a t-test statistics for the explosive drift burst
    hypothesis (Christensen, Oomen and Reno, 2018).

**Finance**

-   The Rmetrics suite of packages comprises
    [fAssets](https://cran.r-project.org/package=fAssets),
    [fBasics](https://cran.r-project.org/package=fBasics),
    [fBonds](https://cran.r-project.org/package=fBonds),
    [timeDate](https://cran.r-project.org/package=timeDate) (formerly: fCalendar),
    [fCopulae](https://cran.r-project.org/package=fCopulae),
    [fExoticOptions](https://cran.r-project.org/package=fExoticOptions),
    [fExtremes](https://cran.r-project.org/package=fExtremes),
    [fGarch](https://cran.r-project.org/package=fGarch),
    [fImport](https://cran.r-project.org/package=fImport),
    [fNonlinear](https://cran.r-project.org/package=fNonlinear),
    [fOptions](https://cran.r-project.org/package=fOptions),
    [fPortfolio](https://cran.r-project.org/package=fPortfolio),
    [fRegression](https://cran.r-project.org/package=fRegression),
    [timeSeries](https://cran.r-project.org/package=timeSeries) (formerly: fSeries),
    [fTrading](https://cran.r-project.org/package=fTrading), and contains a very
    large number of relevant functions for different aspect of empirical
    and computational finance.
-   The [RQuantLib](https://cran.r-project.org/package=RQuantLib) package provides
    several option-pricing functions as well as some fixed-income
    functionality from the QuantLib project to R. The
    [RcppQuantuccia](https://cran.r-project.org/package=RcppQuantuccia) provides a
    smaller subset of QuantLib functionality as a header-only library;
    at current only some calendaring functionality is exposed.
-   The [quantmod](https://cran.r-project.org/package=quantmod) package offers a
    number of functions for quantitative modelling in finance as well as
    data acquisition, plotting and other utilities.
-   The [backtest](https://cran.r-project.org/package=backtest) offers tools to
    explore portfolio-based hypotheses about financial instruments. The
    [pa](https://cran.r-project.org/package=pa) package offers performance
    attribution functionality for equity portfolios.
-   The
    [PerformanceAnalytics](https://cran.r-project.org/package=PerformanceAnalytics)
    package contains a large number of functions for portfolio
    performance calculations and risk management.
-   The [TTR](https://cran.r-project.org/package=TTR) contains functions to
    construct technical trading rules in R.
-   The [sde](https://cran.r-project.org/package=sde) package provides simulation
    and inference functionality for stochastic differential equations.
-   The [YieldCurve](https://cran.r-project.org/package=YieldCurve) package contains
    methods for the estimation of zero-coupon yield curves and spread
    curves based the parametric Nelson and Siegel (1987) method with the
    Svensson (1994) extension. The former package adds the
    McCulloch (1975) cubic splines approach, the latter package adds the
    Diebold and Li approach. The
    [SmithWilsonYieldCurve](https://cran.r-project.org/package=SmithWilsonYieldCurve)
    construct the yield curve using the Smith-Wilson approach based on
    LIBOR and SWAP rates.
-   The [vrtest](https://cran.r-project.org/package=vrtest) package contains a
    number of variance ratio tests for the weak-form of the efficient
    markets hypothesis.
-   The [gmm](https://cran.r-project.org/package=gmm) package provides generalized
    method of moments (GMM) estimations function that are often used
    when estimating the parameters of the moment conditions implied by
    an asset pricing model.
-   The [BurStFin](https://cran.r-project.org/package=BurStFin) and
    [BurStMisc](https://cran.r-project.org/package=BurStMisc) package has a
    collection of function for Finance including the estimation of
    covariance matrices.
-   The [AmericanCallOpt](https://cran.r-project.org/package=AmericanCallOpt)
    package contains a pricer for different American call options.
-   The [VarSwapPrice](https://cran.r-project.org/package=VarSwapPrice) package can
    price a variance swap via a portfolio of European options contracts.
-   The [FinAsym](https://cran.r-project.org/package=FinAsym) package implements the
    Lee and Ready (1991) and Easley and O'Hara (1987) tests for,
    respectively, trade direction, and probability of informed trading.
-   The [parma](https://cran.r-project.org/package=parma) package provides support
    for portfolio allocation and risk management applications.
-   The [GUIDE](https://cran.r-project.org/package=GUIDE) package provides a *GUI*
    for *DE* rivatives and contains numerous pricer examples as well as
    interactive 2d and 3d plots to study these pricing functions.
-   The [SharpeR](https://cran.r-project.org/package=SharpeR) package contains a
    collection of tools for analyzing significance of trading
    strategies, based on the Sharpe ratio and overfit of the same.
-   The [RND](https://cran.r-project.org/package=RND) package implements various
    functions to extract risk-neutral densities from option prices.
-   The [LSMonteCarlo](https://cran.r-project.org/package=LSMonteCarlo) package can
    price American Options via the Least Squares Monte Carlo method.
-   The [BenfordTests](https://cran.r-project.org/package=BenfordTests) package
    provides seven statistical tests and support functions for
    determining if numerical data could conform to Benford's law.
-   The [OptHedging](https://cran.r-project.org/package=OptHedging) package values
    call and put option portfolio and implements an optimal hedging
    strategy.
-   The [markovchain](https://cran.r-project.org/package=markovchain) package
    provides functionality to easily handle and analyse discrete Markov
    chains.
-   The [ycinterextra](https://cran.r-project.org/package=ycinterextra) package
    models yield curve interpolation and extrapolation using via the
    Nelson-Siegel, Svensson, or Smith-Wilson models, as well as Hermite
    cubic splines.
-   The [tvm](https://cran.r-project.org/package=tvm) package models provides
    functions for time value of money such as cashflows and yield
    curves.
-   The [MarkowitzR](https://cran.r-project.org/package=MarkowitzR) package provides
    functions to test the statistical significance of Markowitz
    portfolios.
-   The [pbo](https://cran.r-project.org/package=pbo) package models the probability
    of backtest overfitting, performance degradation, probability of
    loss, and the stochastic dominance when analysing trading
    strategies.
-   The [OptionPricing](https://cran.r-project.org/package=OptionPricing) package
    implements efficient Monte Carlo algorithms for the price and the
    sensitivities of Asian and European Options under Geometric Brownian
    Motion.
-   The [matchingMarkets](https://cran.r-project.org/package=matchingMarkets)
    package implements a structural estimator to correct for the bias
    arising from endogenous matching (e.g. group formation in
    microfinance or matching of firms and venture capitalists).
-   The [restimizeapi](https://cran.r-project.org/package=restimizeapi) package
    interfaces the API at www.estimize.com which provides crowd-sourced
    earnings estimates.
-   The [credule](https://cran.r-project.org/package=credule) package is another
    pricer for credit default swaps.
-   The [obAnalytics](https://cran.r-project.org/package=obAnalytics) package
    analyses and visualizes information from events in limit order book
    data.
-   The [derivmkts](https://cran.r-project.org/package=derivmkts) package adds a set
    of pricing and expository functions useful in teaching derivatives
    markets.
-   The [PortfolioEffectHFT](https://cran.r-project.org/package=PortfolioEffectHFT)
    package provides portfolio analysis suitable for intra-day and
    high-frequency data, and also interfaces the PortfolioEffect
    service.
-   The [ragtop](https://cran.r-project.org/package=ragtop) package prices equity
    derivatives under an extension to Black and Scholes supporting
    default under a power-law link price and hazard rate.
-   The [sharpeRratio](https://cran.r-project.org/package=sharpeRratio) package adds
    moment-free estimation of Sharpe ratios.
-   The [QuantTools](https://cran.r-project.org/package=QuantTools) package offers
    enhanced quantitative trading and modeling tools.
-   The [pinbasic](https://cran.r-project.org/package=pinbasic) package adds tools
    for fast and stable estimates the Probability of Informed Trading
    (PIN) by Easley et al, and offers factorizations of the model
    likelihood. The [InfoTrad](https://cran.r-project.org/package=InfoTrad) packages
    also estimates PIN and extends it different factorization and
    estimation algorithms.
-   The [FinancialMath](https://cran.r-project.org/package=FinancialMath) package
    contains financial math and derivatives pricing functions as
    required by the actuarial exams by the Society of Actuaries and
    Casualty Actuarial Society 'Financial Mathematics' exam.
-   The [tidyquant](https://cran.r-project.org/package=tidyquant) package
    re-arranges functionality from several other key packages for use in
    the so-called tidyverse.
-   The [BCC1997](https://cran.r-project.org/package=BCC1997) prices European
    options under the Bakshi, Cao anc Chen (1997) model for stochastic
    volatility, stochastic rates and random jumps.
-   The [Sim.DiffProc](https://cran.r-project.org/package=Sim.DiffProc) package
    provides functions to simulate and analyse multidimensional Itô and
    Stratonovitch stochastic calculus for continuous-time models.
-   The [BLModel](https://cran.r-project.org/package=BLModel) package computes the
    posterior distribution in a Black-Litterman model from a prior
    distribution given by asset returns and continuous distribution of
    views given by an external function.
-   The [rpatrec](https://cran.r-project.org/package=rpatrec) package aims to
    recognise charting patterns in (financial) time series data.
-   The [PortfolioOptim](https://cran.r-project.org/package=PortfolioOptim) can
    solve both small and large sample portfolio optimization.
-   The [estudy2](https://cran.r-project.org/package=estudy2) package implements
    most commonly used parametric and nonparametric event-study
    methodology tests.
-   The [DtD](https://cran.r-project.org/package=DtD) package computes the *distance
    to default* per Merton's model.
-   The [PeerPerformance](https://cran.r-project.org/package=PeerPerformance)
    package analyzes performance of investments funds relative to its
    peers in a pairwise manner that is robust to false discoveries.
-   The [crseEventStudy](https://cran.r-project.org/package=crseEventStudy) package
    provides another event-study tool to analyse abnormal return in
    long-horizon events.
-   The [simfinapi](https://cran.r-project.org/package=simfinapi) package provides R
    access to [SimFin](https://SimFin.com) fundamental financial
    statement data (given an API key).
-   The [NFCP](https://cran.r-project.org/package=NFCP) package models commodity
    prices via an n-factor term structure estimation.
-   The [LSMRealOptions](https://cran.r-project.org/package=LSMRealOptions) package
    uses least-squares Monte Carlo to value American and Real options.
-   The [AssetCorr](https://cran.r-project.org/package=AssetCorr) package estimates
    intra- and inter-cohort correlations from default data in a Vasicek
    credit portfolio model.
-   The [ichimoku](https://cran.r-project.org/package=ichimoku) package provides
    tools for creating and visualising Ichimoku Kinko Hyo strategies,
    and provides an interface to the OANDA fxTrade API for retrieving
    historical and live streaming price data (which requires free
    registration).
-   The [greeks](https://cran.r-project.org/package=greeks) package calculate
    sensitivities of financial option prices for European and Asian and
    American options in the Black Scholes model.
-   The [RTL](https://cran.r-project.org/package=RTL) (Risk Tool Library) package
    offers a collection of functions and metadata to complement core
    packages in finance and commodities, including futures expiry
    tables.
-   The [GARCHSK](https://cran.r-project.org/package=GARCHSK) package estimates
    GARCHSK and GJRSK models allowing for time-varying volatility,
    skewness and kurtosis.
-   The [bidask](https://cran.r-project.org/package=bidask) package offers a novel
    procedure to estimate bid-ask spreads from OHLC data, and implements
    other reference models.
-   The [strand](https://cran.r-project.org/package=strand) package adds a framework
    for discrete (share-level) simulations of investment strategies.
-   The [HDShOP](https://cran.r-project.org/package=HDShOP) package constructs
    shrinkage estimators of high-dimensional mean-variance portfolios
    and performs high-dimensional tests on optimality, and the
    [DOSPortfolio](https://cran.r-project.org/package=DOSPortfolio) package uses it
    to constructs dynamic optimal shrinkage estimators for the weights
    of the global minimum variance portfolio.

**Risk management**

-   The packages [qrmtools](https://cran.r-project.org/package=qrmtools) and
    [qrmdata](https://cran.r-project.org/package=qrmdata) provide tools and data for
    standard tasks in Quantitative Risk Management (QRM) and accompany
    the book of [McNeil, Frey, Embrechts (2005, 2015, "Quantitative Risk
    Management: Concepts, Techniques,
    Tools")](https://press.princeton.edu/books/hardcover/9780691166278/quantitative-risk-management)
    .
-   The Task View
    [ExtremeValue](https://cran.r-project.org/web/views/ExtremeValue.html)
    regroups a number of relevant packages.
-   The packages [CreditMetrics](https://cran.r-project.org/package=CreditMetrics)
    provides function for modelling credit risks.
-   The [mvtnorm](https://cran.r-project.org/package=mvtnorm) package provides code
    for multivariate Normal and t-distributions.
-   The package [nvmix](https://cran.r-project.org/package=nvmix) provides
    functionality for multivariate normal variance mixtures (including
    normal and t for non-integer degrees of freedom).
-   The Rmetrics packages
    [fPortfolio](https://cran.r-project.org/package=fPortfolio) and
    [fExtremes](https://cran.r-project.org/package=fExtremes) also contain a number
    of relevant functions.
-   The packages [copula](https://cran.r-project.org/package=copula) and
    [copulaData](https://cran.r-project.org/package=copulaData) cover a wide range
    of modeling tasks for copulas.
-   The [fgac](https://cran.r-project.org/package=fgac) package implements
    generalized Archimedean copulas.
-   The [actuar](https://cran.r-project.org/package=actuar) package provides an
    actuarial perspective to risk management.
-   The [ghyp](https://cran.r-project.org/package=ghyp) package provides generalized
    hyberbolic distribution functions as well as procedures for VaR,
    CVaR or target-return portfolio optimizations.
-   The [ChainLadder](https://cran.r-project.org/package=ChainLadder) package
    provides functions for modeling insurance claim reserves; and the
    [lifecontingencies](https://cran.r-project.org/package=lifecontingencies)
    package provides functions for financial and actuarial evaluations
    of life contingencies.
-   The [frmqa](https://cran.r-project.org/package=frmqa) package aims to collect
    functions for Financial Risk Management and Quantitative Analysis.
-   The [ESG](https://cran.r-project.org/package=ESG) package can be used to model
    for asset projection, a scenario-based simulation approach.
-   The [riskSimul](https://cran.r-project.org/package=riskSimul) package provides
    efficient simulation procedures to estimate tail loss probabilities
    and conditional excess for a stock portfolios where log-returns are
    assumed to follow a t-copula model with generalized hyperbolic or t
    marginals.
-   The [GCPM](https://cran.r-project.org/package=GCPM) package analyzes the default
    risk of credit portfolio using both analytical and simulation
    approaches.
-   The [FatTailsR](https://cran.r-project.org/package=FatTailsR) package provides a
    family of four distributions tailored to distribution with symmetric
    and asymmetric fat tails.
-   The [Dowd](https://cran.r-project.org/package=Dowd) package contains functions
    ported from the 'MMR2' toolbox offered in Kevin Dowd's book
    "Measuring Market Risk".
-   The [PortRisk](https://cran.r-project.org/package=PortRisk) package computes
    portfolio risk attribution.
-   The
    [NetworkRiskMeasures](https://cran.r-project.org/package=NetworkRiskMeasures)
    package implements some risk measures for financial networks such as
    DebtRank, Impact Susceptibility, Impact Diffusion and Impact
    Fluidity.
-   The [Risk](https://cran.r-project.org/package=Risk) package computes 26
    financial risk measures for any continuous distribution.
-   The [RiskPortfolios](https://cran.r-project.org/package=RiskPortfolios) package
    constructs risk-based portfolios as per the corresponding papers by
    Ardia et al.
-   The [reinsureR](https://cran.r-project.org/package=reinsureR) package models
    reinsurances a class Claims whose objective is to store claims and
    premiums, on which different treaties can be applied.
-   The [RM2006](https://cran.r-project.org/package=RM2006) package estimates
    conditional covariance matrix using the RiskMetrics 2006 methodology
    described in Zumbach (2007).
-   The [cvar](https://cran.r-project.org/package=cvar) package computes expected
    shortfall and value at risk for continuous distributions.
-   [riskParityPortfolio](https://cran.r-project.org/package=riskParityPortfolio)
    offers fast implementations for constructing risk-parity portfolios.
-   The [monobin](https://cran.r-project.org/package=monobin) package performs
    monotonic binning of numeric risk factor in credit rating models
    (PD, LGD, EAD) development.
-   The [etrm](https://cran.r-project.org/package=etrm) package contains a
    collection of functions to perform core tasks within energy trading
    and risk management (ETRM).

**Books**

-   The [NMOF](https://cran.r-project.org/package=NMOF) package provides functions,
    examples and data from *Numerical Methods and Optimization in
    Finance* by Manfred Gilli, Dietmar Maringer and Enrico Schumann
    (2011), including the different optimization heuristics such as
    Differential Evolution, Genetic Algorithms, Particle Swarms, and
    Threshold Accepting.
-   The [FRAPO](https://cran.r-project.org/package=FRAPO) package provides data sets
    and code for the book *Financial Risk Modelling and Portfolio
    Optimization with R* by Bernhard Pfaff (2013).

**Data and date management**

-   The [zoo](https://cran.r-project.org/package=zoo) and
    [timeDate](https://cran.r-project.org/package=timeDate) (part of Rmetrics)
    packages provide support for irregularly-spaced time series. The
    [xts](https://cran.r-project.org/package=xts) package extends
    [zoo](https://cran.r-project.org/package=zoo) specifically for financial time
    series. See the
    [TimeSeries](https://cran.r-project.org/web/views/TimeSeries.html)
    task view for more details.
-   [timeDate](https://cran.r-project.org/package=timeDate) also addresses calendar
    issues such as recurring holidays for a large number of financial
    centers, and provides code for high-frequency data sets.
-   The [fame](https://cran.r-project.org/package=fame) package can access Fame time
    series databases (but also requires a Fame backend). The
    [tis](https://cran.r-project.org/package=tis) package provides time indices and
    time-indexed series compatible with Fame frequencies.
-   The [TSdbi](https://cran.r-project.org/package=TSdbi) package provides a
    unifying interface for several time series data base backends, and
    its SQL implementations provide a database table design.
-   The [IBrokers](https://cran.r-project.org/package=IBrokers) package provides
    access to the Interactive Brokers API for data access (but requires
    an account to access the service).
-   The [data.table](https://cran.r-project.org/package=data.table) package provides
    very efficient and fast access to in-memory data sets such as asset
    prices.
-   The [TFX](https://cran.r-project.org/package=TFX) package provides an interface
    to the TrueFX (TM) service for free streaming real-time and
    historical tick-by-tick market data for interbank foreign exchange
    rates at the millisecond resolution.
-   The package [highfrequency](https://cran.r-project.org/package=highfrequency)
    contains functionality to manage, clean and match highfrequency
    trades and quotes data and enables users to calculate various
    liquidity measures, estimate and forecast volatility, and
    investigate microstructure noise and intraday periodicity.
-   The [Rbitcoin](https://cran.r-project.org/package=Rbitcoin) package offers
    access to Bitcoin exchange APIs (mtgox, bitstamp, btce, kraken) via
    public and private API calls and integration of data structures for
    all markets.
-   The [bizdays](https://cran.r-project.org/package=bizdays) package compute
    business days if provided a list of holidays.
-   The [TAQMNGR](https://cran.r-project.org/package=TAQMNGR) package manages
    tick-by-tick (equity) transaction data performing 'cleaning',
    'aggregation' and 'import' where cleaning and aggregation are
    performed according to Brownlees and Gallo (2006).
-   The [Rblpapi](https://cran.r-project.org/package=Rblpapi) package offers
    efficient access to the Bloomberg API and allows bdp, bdh, and bds
    queries as well as data retrieval both in (regular time-)bars and
    ticks (albeit without subsecond resolution).
-   The [finreportr](https://cran.r-project.org/package=finreportr) package can
    download reports from the SEC Edgar database, and relies on, inter
    alia, the [XBRL](https://cran.r-project.org/package=XBRL) package for parsing
    these reports.
-   The [GetTDData](https://cran.r-project.org/package=GetTDData) package imports
    Brazilian government bonds data (such as LTN, NTN-B and LFT ) from
    the Tesouro Direto website.
-   The [fmdates](https://cran.r-project.org/package=fmdates) package implements
    common date calculations according to the ISDA schedules, and can
    check for business in different locales.
-   Data from Kenneth French's website can be downloaded with packages
    [FFdownload](https://cran.r-project.org/package=FFdownload) and
    [frenchdata](https://cran.r-project.org/package=frenchdata). Individual datasets
    can also be downloaded with function French in package
    [NMOF](https://cran.r-project.org/package=NMOF).

</div>

### CRAN packages:

-   [actuar](https://cran.r-project.org/package=actuar)
-   [AmericanCallOpt](https://cran.r-project.org/package=AmericanCallOpt)
-   [AssetCorr](https://cran.r-project.org/package=AssetCorr)
-   [backtest](https://cran.r-project.org/package=backtest)
-   [bayesGARCH](https://cran.r-project.org/package=bayesGARCH)
-   [BCC1997](https://cran.r-project.org/package=BCC1997)
-   [BenfordTests](https://cran.r-project.org/package=BenfordTests)
-   [betategarch](https://cran.r-project.org/package=betategarch)
-   [bidask](https://cran.r-project.org/package=bidask)
-   [bizdays](https://cran.r-project.org/package=bizdays)
-   [BLModel](https://cran.r-project.org/package=BLModel)
-   [bmgarch](https://cran.r-project.org/package=bmgarch)
-   [BurStFin](https://cran.r-project.org/package=BurStFin)
-   [BurStMisc](https://cran.r-project.org/package=BurStMisc)
-   [CADFtest](https://cran.r-project.org/package=CADFtest)
-   [car](https://cran.r-project.org/package=car)
-   [ChainLadder](https://cran.r-project.org/package=ChainLadder)
-   [copula](https://cran.r-project.org/package=copula)
-   [copulaData](https://cran.r-project.org/package=copulaData)
-   [CreditMetrics](https://cran.r-project.org/package=CreditMetrics)
-   [credule](https://cran.r-project.org/package=credule)
-   [crseEventStudy](https://cran.r-project.org/package=crseEventStudy)
-   [cvar](https://cran.r-project.org/package=cvar)
-   [data.table](https://cran.r-project.org/package=data.table)
-   [derivmkts](https://cran.r-project.org/package=derivmkts)
-   [dlm](https://cran.r-project.org/package=dlm)
-   [DOSPortfolio](https://cran.r-project.org/package=DOSPortfolio)
-   [Dowd](https://cran.r-project.org/package=Dowd)
-   [DriftBurstHypothesis](https://cran.r-project.org/package=DriftBurstHypothesis)
-   [dse](https://cran.r-project.org/package=dse)
-   [DtD](https://cran.r-project.org/package=DtD)
-   [dyn](https://cran.r-project.org/package=dyn)
-   [dynlm](https://cran.r-project.org/package=dynlm)
-   [ESG](https://cran.r-project.org/package=ESG)
-   [estudy2](https://cran.r-project.org/package=estudy2)
-   [etrm](https://cran.r-project.org/package=etrm)
-   [factorstochvol](https://cran.r-project.org/package=factorstochvol)
-   [fame](https://cran.r-project.org/package=fame)
-   [fAssets](https://cran.r-project.org/package=fAssets) (core)
-   [FatTailsR](https://cran.r-project.org/package=FatTailsR)
-   [fBasics](https://cran.r-project.org/package=fBasics) (core)
-   [fBonds](https://cran.r-project.org/package=fBonds) (core)
-   [fCopulae](https://cran.r-project.org/package=fCopulae) (core)
-   [fExoticOptions](https://cran.r-project.org/package=fExoticOptions) (core)
-   [fExtremes](https://cran.r-project.org/package=fExtremes) (core)
-   [FFdownload](https://cran.r-project.org/package=FFdownload)
-   [fgac](https://cran.r-project.org/package=fgac)
-   [fGarch](https://cran.r-project.org/package=fGarch) (core)
-   [fImport](https://cran.r-project.org/package=fImport) (core)
-   [FinancialMath](https://cran.r-project.org/package=FinancialMath)
-   [FinAsym](https://cran.r-project.org/package=FinAsym)
-   [finreportr](https://cran.r-project.org/package=finreportr)
-   [fmdates](https://cran.r-project.org/package=fmdates)
-   [fMultivar](https://cran.r-project.org/package=fMultivar) (core)
-   [fNonlinear](https://cran.r-project.org/package=fNonlinear) (core)
-   [fOptions](https://cran.r-project.org/package=fOptions) (core)
-   [forecast](https://cran.r-project.org/package=forecast)
-   [fPortfolio](https://cran.r-project.org/package=fPortfolio) (core)
-   [fracdiff](https://cran.r-project.org/package=fracdiff)
-   [FRAPO](https://cran.r-project.org/package=FRAPO)
-   [fRegression](https://cran.r-project.org/package=fRegression) (core)
-   [frenchdata](https://cran.r-project.org/package=frenchdata)
-   [frmqa](https://cran.r-project.org/package=frmqa)
-   [fTrading](https://cran.r-project.org/package=fTrading) (core)
-   [garchmodels](https://cran.r-project.org/package=garchmodels)
-   [garchx](https://cran.r-project.org/package=garchx)
-   [GCPM](https://cran.r-project.org/package=GCPM)
-   [gets](https://cran.r-project.org/package=gets)
-   [GetTDData](https://cran.r-project.org/package=GetTDData)
-   [ghyp](https://cran.r-project.org/package=ghyp)
-   [gmm](https://cran.r-project.org/package=gmm)
-   [gogarch](https://cran.r-project.org/package=gogarch)
-   [greeks](https://cran.r-project.org/package=greeks)
-   [GUIDE](https://cran.r-project.org/package=GUIDE)
-   [HDShOP](https://cran.r-project.org/package=HDShOP)
-   [highfrequency](https://cran.r-project.org/package=highfrequency)
-   [IBrokers](https://cran.r-project.org/package=IBrokers)
-   [ichimoku](https://cran.r-project.org/package=ichimoku)
-   [InfoTrad](https://cran.r-project.org/package=InfoTrad)
-   [lgarch](https://cran.r-project.org/package=lgarch)
-   [lifecontingencies](https://cran.r-project.org/package=lifecontingencies)
-   [lmtest](https://cran.r-project.org/package=lmtest)
-   [longmemo](https://cran.r-project.org/package=longmemo)
-   [LSMonteCarlo](https://cran.r-project.org/package=LSMonteCarlo)
-   [LSMRealOptions](https://cran.r-project.org/package=LSMRealOptions)
-   [markovchain](https://cran.r-project.org/package=markovchain)
-   [MarkowitzR](https://cran.r-project.org/package=MarkowitzR)
-   [matchingMarkets](https://cran.r-project.org/package=matchingMarkets)
-   [monobin](https://cran.r-project.org/package=monobin)
-   [MSGARCH](https://cran.r-project.org/package=MSGARCH)
-   [mvtnorm](https://cran.r-project.org/package=mvtnorm)
-   [NetworkRiskMeasures](https://cran.r-project.org/package=NetworkRiskMeasures)
-   [NFCP](https://cran.r-project.org/package=NFCP)
-   [nlme](https://cran.r-project.org/package=nlme)
-   [NMOF](https://cran.r-project.org/package=NMOF)
-   [nvmix](https://cran.r-project.org/package=nvmix)
-   [obAnalytics](https://cran.r-project.org/package=obAnalytics)
-   [OptHedging](https://cran.r-project.org/package=OptHedging)
-   [OptionPricing](https://cran.r-project.org/package=OptionPricing)
-   [pa](https://cran.r-project.org/package=pa)
-   [parma](https://cran.r-project.org/package=parma)
-   [pbo](https://cran.r-project.org/package=pbo)
-   [PeerPerformance](https://cran.r-project.org/package=PeerPerformance)
-   [PerformanceAnalytics](https://cran.r-project.org/package=PerformanceAnalytics)
    (core)
-   [pinbasic](https://cran.r-project.org/package=pinbasic)
-   [PortfolioEffectHFT](https://cran.r-project.org/package=PortfolioEffectHFT)
-   [PortfolioOptim](https://cran.r-project.org/package=PortfolioOptim)
-   [PortRisk](https://cran.r-project.org/package=PortRisk)
-   [qrmdata](https://cran.r-project.org/package=qrmdata)
-   [qrmtools](https://cran.r-project.org/package=qrmtools)
-   [quantmod](https://cran.r-project.org/package=quantmod)
-   [QuantTools](https://cran.r-project.org/package=QuantTools)
-   [ragtop](https://cran.r-project.org/package=ragtop)
-   [Rbitcoin](https://cran.r-project.org/package=Rbitcoin)
-   [Rblpapi](https://cran.r-project.org/package=Rblpapi)
-   [Rcmdr](https://cran.r-project.org/package=Rcmdr)
-   [RcppQuantuccia](https://cran.r-project.org/package=RcppQuantuccia)
-   [reinsureR](https://cran.r-project.org/package=reinsureR)
-   [restimizeapi](https://cran.r-project.org/package=restimizeapi)
-   [Risk](https://cran.r-project.org/package=Risk)
-   [riskParityPortfolio](https://cran.r-project.org/package=riskParityPortfolio)
-   [RiskPortfolios](https://cran.r-project.org/package=RiskPortfolios)
-   [riskSimul](https://cran.r-project.org/package=riskSimul)
-   [RM2006](https://cran.r-project.org/package=RM2006)
-   [rmgarch](https://cran.r-project.org/package=rmgarch)
-   [RND](https://cran.r-project.org/package=RND)
-   [rpatrec](https://cran.r-project.org/package=rpatrec)
-   [RQuantLib](https://cran.r-project.org/package=RQuantLib)
-   [RTL](https://cran.r-project.org/package=RTL)
-   [rugarch](https://cran.r-project.org/package=rugarch) (core)
-   [rwt](https://cran.r-project.org/package=rwt)
-   [sandwich](https://cran.r-project.org/package=sandwich)
-   [sde](https://cran.r-project.org/package=sde)
-   [SharpeR](https://cran.r-project.org/package=SharpeR)
-   [sharpeRratio](https://cran.r-project.org/package=sharpeRratio)
-   [Sim.DiffProc](https://cran.r-project.org/package=Sim.DiffProc)
-   [simfinapi](https://cran.r-project.org/package=simfinapi)
-   [SmithWilsonYieldCurve](https://cran.r-project.org/package=SmithWilsonYieldCurve)
-   [stochvol](https://cran.r-project.org/package=stochvol)
-   [strand](https://cran.r-project.org/package=strand)
-   [strucchange](https://cran.r-project.org/package=strucchange)
-   [TAQMNGR](https://cran.r-project.org/package=TAQMNGR)
-   [TFX](https://cran.r-project.org/package=TFX)
-   [tidyquant](https://cran.r-project.org/package=tidyquant)
-   [timeDate](https://cran.r-project.org/package=timeDate) (core)
-   [timeSeries](https://cran.r-project.org/package=timeSeries) (core)
-   [timsac](https://cran.r-project.org/package=timsac)
-   [tis](https://cran.r-project.org/package=tis)
-   [TSdbi](https://cran.r-project.org/package=TSdbi)
-   [tsDyn](https://cran.r-project.org/package=tsDyn)
-   [tseries](https://cran.r-project.org/package=tseries) (core)
-   [tseriesChaos](https://cran.r-project.org/package=tseriesChaos)
-   [TTR](https://cran.r-project.org/package=TTR)
-   [tvm](https://cran.r-project.org/package=tvm)
-   [urca](https://cran.r-project.org/package=urca) (core)
-   [vars](https://cran.r-project.org/package=vars)
-   [VarSwapPrice](https://cran.r-project.org/package=VarSwapPrice)
-   [vrtest](https://cran.r-project.org/package=vrtest)
-   [wavelets](https://cran.r-project.org/package=wavelets)
-   [waveslim](https://cran.r-project.org/package=waveslim)
-   [wavethresh](https://cran.r-project.org/package=wavethresh)
-   [XBRL](https://cran.r-project.org/package=XBRL)
-   [xts](https://cran.r-project.org/package=xts) (core)
-   [ycinterextra](https://cran.r-project.org/package=ycinterextra)
-   [YieldCurve](https://cran.r-project.org/package=YieldCurve)
-   [zoo](https://cran.r-project.org/package=zoo) (core)

### Related links:

-   CRAN Task View: [Econometrics](Econometrics.html)
-   CRAN Task View: [ExtremeValue](ExtremeValue.html)
-   CRAN Task View: [Multivariate](Multivariate.html)
-   CRAN Task View: [Optimization](Optimization.html)
-   CRAN Task View: [Robust](Robust.html)
-   CRAN Task View: [SocialSciences](SocialSciences.html)
-   CRAN Task View: [TimeSeries](TimeSeries.html)
-   [Rmetrics contains a wealth of R code for
    Finance](http://www.rmetrics.org)
-   [Quantlib is a C++ library for quantitative
    finance](http://www.quantlib.org)
-   [Documentation for the Bloomberg API accessed by
    Rblpapi](http://www.bloomberglabs.com//)
-   [Mailing list: R Special Interest Group
    Finance](https://stat.ethz.ch/mailman/listinfo/R-SIG-Finance/)
-   [MSCI indexes data](http://www.msci.com/)
-   [French/Fama
    data](http://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)
-   [Wilshire indexes data](http://www.wilshire.com/Indexes/calculator/)
-   [Rene
    Carmona](http://orfe.princeton.edu/~rcarmona/maindownload.html)
-   [Eric Zivot](http://faculty.washington.edu/ezivot/splus.htm)
-   [R Code for Ruppert's 'Statistics and
    Finance'](http://christopherggreen.github.io/RuppertStatisticsFinance2004/)
-   [Guy Yollin](http://www.r-programming.org/papers)
-   [GitHub repository for this Task
    View](https://github.com/eddelbuettel/ctv-finance)
