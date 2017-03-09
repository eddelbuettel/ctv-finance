CRAN Task View: Empirical Finance
---------------------------------

|                 |                                             
|-----------------|-------------------------------------------  
| **Maintainer:** | Dirk Eddelbuettel                           
| **Contact:**    | Dirk.Eddelbuettel at R-project.org          
| **Version:**    | 2017-03-07                                  
| **URL:**        | <https://CRAN.R-project.org/view=Finance>   

This CRAN Task View contains a list of packages useful for empirical work in Finance, grouped by topic.

Besides these packages, a very wide variety of functions suitable for empirical work in Finance is provided by both the basic R system (and its set of recommended core packages), and a number of other packages on the Comprehensive R Archive Network (CRAN). Consequently, several of the other CRAN Task Views may contain suitable packages, in particular the [Econometrics](https://cran.r-project.org/web/views/Econometrics.html), [Multivariate](https://cran.r-project.org/web/views/Multivariate.html), [Optimization](https://cran.r-project.org/web/views/Optimization.html), [Robust](https://cran.r-project.org/web/views/Robust.html), [SocialSciences](https://cran.r-project.org/web/views/SocialSciences.html) and [TimeSeries](https://cran.r-project.org/web/views/TimeSeries.html) Task Views.

Contributions are always welcome, and encouraged. Since the start of this CRAN task view in April 2005, most contributions have arrived as email suggestions. The source file for this particular task view file now also reside in a GitHub repository (see below) so that pull requests are also possible.

The [ctv](https://cran.r-project.org/package=ctv) package supports these Task Views. Its functions `install.views` and `update.views` allow, respectively, installation or update of packages from a given Task View; the option `coreOnly` can restrict operations to packages labeled as *core* below.

**Standard regression models**

-   A detailed overview of the available regression methodologies is provided by the [Econometrics](https://cran.r-project.org/web/views/Econometrics.html) task view. This is complemented by the [Robust](https://cran.r-project.org/web/views/Robust.html) task view, which focuses on more robust and resistant methods.
-   Linear models such as ordinary least squares (OLS) can be estimated by `lm()` (from by the stats package contained in the basic R distribution). Maximum Likelihood (ML) estimation can be undertaken with the standard `optim()` function. Many other suitable methods are listed in the [Optimization](https://cran.r-project.org/web/views/Optimization.html) view. Non-linear least squares can be estimated with the `nls()` function, as well as with `nlme()` from the [nlme](https://cran.r-project.org/package=nlme) package.
-   For the linear model, a variety of regression diagnostic tests are provided by the [car](https://cran.r-project.org/package=car/index.html), [lmtest](../packages/lmtest/index.html), [strucchange](../packages/strucchange/index.html), [urca](../packages/urca/index.html), and [sandwich](../packages/sandwich/index.html) packages. The [Rcmdr](../packages/Rcmdr/index.html) and [Zelig](../packages/Zelig) packages provide user interfaces that may be of interest as well.

**Time series**

-   A detailed overview of tools for time series analysis can be found in the [TimeSeries](https://cran.r-project.org/web/views/TimeSeries.html) task view. Below a brief overview of the most important methods in finance is given.
-   Classical time series functionality is provided by the `arima()` and `KalmanLike()` commands in the basic R distribution.
-   The [dse](https://cran.r-project.org/package=dse/index.html) and [timsac](../packages/timsac/index.html) packages provide a variety of more advanced estimation methods; [fracdiff](../packages/fracdiff/index.html) can estimate fractionally integrated series; [longmemo](../packages/longmemo/index.html) covers related material. The [fractal](../packages/fractal) provide fractal time series modeling functionality.
-   For volatility modeling, the standard GARCH(1,1) model can be estimated with the `garch()` function in the [tseries](https://cran.r-project.org/package=tseries/index.html) package. Rmetrics (see below) contains the [fGarch](../packages/fGarch/index.html) package which has additional models. The [rugarch](../packages/rugarch/index.html) package can be used to model a variety of univariate GARCH models with extensions such as ARFIMA, in-mean, external regressors and various other specifications; with methods for fit, forecast, simulation, inference and plotting are provided too. The [rmgarch](../packages/rmgarch/index.html) builds on it to provide the ability to estimate several multivariate GARCH models. The [betategarch](../packages/betategarch/index.html) package can estimate and simulate the Beta-t-EGARCH model by Harvey. The [bayesGARCH](../packages/bayesGARCH/index.html) package can perform Bayesian estimation of a GARCH(1,1) model with Student's t innovations. For multivariate models, the [ccgarch](../packages/ccgarch/index.html) package can estimate (multivariate) Conditional Correlation GARCH models whereas the [gogarch](../packages/gogarch/index.html) package provides functions for generalized orthogonal GARCH models. The [gets](../packages/gets/index.html) package (which was preceded by a related package AutoSEARCH) provides automated general-to-specific model selection of the mean and log-volatility of a log-ARCH-X model. The [GEVStableGarch](../packages/GEVStableGarch/index.html) package can fit ARMA-GARCH or ARMA-APARCH models with GEV and stable conditional distributions. The [lgarch](../packages/lgarch) package can estimate and fit log-Garch models.
-   Unit root and cointegration tests are provided by [tseries](https://cran.r-project.org/package=tseries/index.html), and [urca](../packages/urca/index.html). The Rmetrics packages [timeSeries](../packages/timeSeries/index.html) and [fMultivar](../packages/fMultivar/index.html) contain a number of estimation functions for ARMA, GARCH, long memory models, unit roots and more. The [CADFtest](../packages/CADFtest) package implements the Hansen unit root test.
-   [MSBVAR](https://cran.r-project.org/package=MSBVAR/index.html) provides Bayesian estimation of vector autoregressive models. The [dlm](../packages/dlm) package provides Bayesian and likelihood analysis of dynamic linear models (ie linear Gaussian state space models).
-   The [vars](https://cran.r-project.org/package=vars) package offer estimation, diagnostics, forecasting and error decomposition of VAR and SVAR model in a classical framework.
-   The [dyn](https://cran.r-project.org/package=dyn/index.html) and [dynlm](../packages/dynlm) packages are suitable for dynamic (linear) regression models.
-   Several packages provide wavelet analysis functionality: [rwt](https://cran.r-project.org/package=rwt/index.html), [wavelets](../packages/wavelets/index.html), [waveslim](../packages/waveslim/index.html), [wavethresh](../packages/wavethresh/index.html). Some methods from chaos theory are provided by the package [tseriesChaos](../packages/tseriesChaos/index.html). [tsDyn](../packages/tsDyn) adds time series analysis based on dynamical systems therory.
-   The [forecast](https://cran.r-project.org/package=forecast) package adds functions for forecasting problems.
-   The [tsfa](https://cran.r-project.org/package=tsfa) package provides functions for time series factor analysis.
-   The [stochvol](https://cran.r-project.org/package=stochvol/index.html) package implements Bayesian estimation of stochastic volatility using Markov Chain Monte Carlo, and [factorstochvol](../packages/factorstochvol) extends this to the multivariate case.
-   The [MSGARCH](https://cran.r-project.org/package=MSGARCH) package adds methods to fit (by Maximum Likelihood or Bayesian), simulate, and forecast various Markov-Switching GARCH processes.

**Finance**

-   The Rmetrics suite of packages comprises [fArma](https://cran.r-project.org/package=fArma/index.html), [fAsianOptions](../packages/fAsianOptions/index.html), [fAssets](../packages/fAssets/index.html), [fBasics](../packages/fBasics/index.html), [fBonds](../packages/fBonds/index.html), [timeDate](../packages/timeDate/index.html) (formerly: fCalendar), [fCopulae](../packages/fCopulae/index.html), [fExoticOptions](../packages/fExoticOptions/index.html), [fExtremes](../packages/fExtremes/index.html), [fGarch](../packages/fGarch/index.html), [fImport](../packages/fImport/index.html), [fNonlinear](../packages/fNonlinear/index.html), [fOptions](../packages/fOptions/index.html), [fPortfolio](../packages/fPortfolio/index.html), [fRegression](../packages/fRegression/index.html), [timeSeries](../packages/timeSeries/index.html) (formerly: fSeries), [fTrading](../packages/fTrading/index.html), [fUnitRoots](../packages/fUnitRoots) and contains a very large number of relevant functions for different aspect of empirical and computational finance.
-   The [RQuantLib](https://cran.r-project.org/package=RQuantLib) package provides several option-pricing functions as well as some fixed-income functionality from the QuantLib project to R.
-   The [quantmod](https://cran.r-project.org/package=quantmod) package offers a number of functions for quantitative modelling in finance as well as data acqusition, plotting and other utilities.
-   The [portfolio](https://cran.r-project.org/package=portfolio/index.html) package contains classes for equity portfolio management; the [portfolioSim](../packages/portfolioSim/index.html) builds a related simulation framework. The [backtest](../packages/backtest/index.html) offers tools to explore portfolio-based hypotheses about financial instruments. The [stockPortfolio](../packages/stockPortfolio/index.html) package provides functions for single index, constant correlation and multigroup models. The [pa](../packages/pa) package offers performance attribution functionality for equity portfolios.
-   The [PerformanceAnalytics](https://cran.r-project.org/package=PerformanceAnalytics) package contains a large number of functions for portfolio performance calculations and risk management.
-   The [TTR](https://cran.r-project.org/package=TTR) contains functions to construct technical trading rules in R.
-   The [financial](https://cran.r-project.org/package=financial) package can compute present values, cash flows and other simple finance calculations.
-   The [sde](https://cran.r-project.org/package=sde) package provides simulation and inference functionality for stochastic differential equations.
-   The [termstrc](https://cran.r-project.org/package=termstrc/index.html) and [YieldCurve](../packages/YieldCurve/index.html) packages contain methods for the estimation of zero-coupon yield curves and spread curves based the parametric Nelson and Siegel (1987) method with the Svensson (1994) extension. The former package adds the McCulloch (1975) cubic splines approach, the latter package adds the Diebold and Li approach. The [SmithWilsonYieldCurve](../packages/SmithWilsonYieldCurve) construct the yield curve using the Smith-Wilson approach based on LIBOR and SWAP rates.
-   The [vrtest](https://cran.r-project.org/package=vrtest) package contains a number of variance ratio tests for the weak-form of the efficient markets hypothesis.
-   The [gmm](https://cran.r-project.org/package=gmm) package provides generalized method of moments (GMM) estimations function that are often used when estimating the parameters of the moment conditions implied by an asset pricing model.
-   The [tawny](https://cran.r-project.org/package=tawny) package contains estimator based on random matrix theory as well as shrinkage methods to remove sampling noise when estimating sample covariance matrices.
-   The [opefimor](https://cran.r-project.org/package=opefimor) package by contains material to accompany the Iacus (2011) book entitled "Option Pricing and Estimation of Financial Models in R".
-   The [maRketSim](https://cran.r-project.org/package=maRketSim) package provides a market simulator, initially designed around the bond market.
-   The [BurStFin](https://cran.r-project.org/package=BurStFin/index.html) and [BurStMisc](../packages/BurStMisc) package has a collection of function for Finance including the estimation of covariance matrices.
-   The [AmericanCallOpt](https://cran.r-project.org/package=AmericanCallOpt) package contains a pricer for different American call options.
-   The [VarSwapPrice](https://cran.r-project.org/package=VarSwapPrice) package can price a variance swap via a portfolio of European options contracts.
-   The [FinAsym](https://cran.r-project.org/package=FinAsym) package implements the Lee and Ready (1991) and Easley and O'Hara (1987) tests for, respectively, trade direction, and probability of informed trading.
-   The [parma](https://cran.r-project.org/package=parma) package provides support for portfolio allocation and risk management applications.
-   The [GUIDE](https://cran.r-project.org/package=GUIDE) package provides a *GUI* for *DE* rivatives and contains numerous pricer examples as well as interactive 2d and 3d plots to study these pricing functions.
-   The [SharpeR](https://cran.r-project.org/package=SharpeR) package contains a collection of tools for analyzing significance of trading strategies, based on the Sharpe ratio and overfit of the same.
-   The [RND](https://cran.r-project.org/package=RND) package implements various functions to extract risk-neutral densities from option prices.
-   [LSMonteCarlo](https://cran.r-project.org/package=LSMonteCarlo) can price American Options via the Least Squares Monte Carlo method
-   The [BenfordTests](https://cran.r-project.org/package=BenfordTests) package provides seven statistical tests and support functions for determining if numerical data could conform to Benford's law.
-   The [OptHedging](https://cran.r-project.org/package=OptHedging) package values call and put option portfolio and implements an optimal hedging strategy.
-   The [markovchain](https://cran.r-project.org/package=markovchain) package provides functionality to easily handle and analyse discrete Markov chains.
-   The [ycinterextra](https://cran.r-project.org/package=ycinterextra) package models yield curve interpolation and extrapolation using via the Nelson-Siegel, Svensson, or Smith-Wilson models, as well as Hermite cubic splines.
-   The [tvm](https://cran.r-project.org/package=tvm) package models provides functions for time value of money such as cashflows and yield curves.
-   The [MarkowitzR](https://cran.r-project.org/package=MarkowitzR) package provides functions to test the statistical signicance of Markowitz portfolios.
-   The [egcm](https://cran.r-project.org/package=egcm) package implements the Engle-Granger two-stage cointegration modeling procedure with a particular focus on pairs trading.
-   The [pbo](https://cran.r-project.org/package=pbo) package models the probability of backtest overfitting, performance degradation, probability of loss, and the stochastic dominance when analysing trading strategies.
-   The [OptionPricing](https://cran.r-project.org/package=OptionPricing) package implements efficient Monte Carlo algorithms for the price and the sensitivities of Asian and European Options under Geometric Brownian Motion.
-   The [matchingMarkets](https://cran.r-project.org/package=matchingMarkets) package implements a structural estimator to correct for the bias arising from endogenous matching (e.g. group formation in microfinance or matching of firms and venture capitalists).
-   The [restimizeapi](https://cran.r-project.org/package=restimizeapi) package interfaces the API at www.estimize.com which provides crowd-sourced earnings estimates.
-   The [credule](https://cran.r-project.org/package=credule) package is another pricer for credit default swaps.
-   The [covmat](https://cran.r-project.org/package=covmat) package provides several different methods for computing covariance matrices.
-   The [obAnalytics](https://cran.r-project.org/package=obAnalytics) package analyses and visualizes information from events in limit order book data.
-   The [bootTimeInference](https://cran.r-project.org/package=bootTimeInference) package performs robust resampling tests for the difference in Sharpe ratios.
-   The [derivmkts](https://cran.r-project.org/package=derivmkts) package adds a set of pricing and expository functions useful in teaching derivatives markets..
-   The [PortfolioEffectHFT](https://cran.r-project.org/package=PortfolioEffectHFT) package provides portfolio analysis suitable for intra-day and high-frequency data, and also interfaces the PortfolioEffect service.
-   The [ragtop](https://cran.r-project.org/package=ragtop) package prices equity derivatives under an extension to Black and Scholes supporting default under a power-law link price and hazard rate.
-   The [sharpeRratio](https://cran.r-project.org/package=sharpeRratio) package adds moment-free estimation of Sharpe ratios.
-   The [QuantTools](https://cran.r-project.org/package=QuantTools) package offers enhanced quantitative trading and modeling tools.
-   The [pinbasic](https://cran.r-project.org/package=pinbasic/index.html) package adds tools for fast and stable estimates the Probability of Informed Trading (PIN) by Easley et al, and offers factorizations of the model likelihood. The [InfoTrad](../packages/InfoTrad) packages also estimates PIN and extends it different factorization and estimation algorithms.
-   The [FinancialMath](https://cran.r-project.org/package=FinancialMath) package contains financial math and derivatives pricing functions as required by the actuarial exams by the Society of Actuaries and Casualty Actuarial Society 'Financial Mathematics' exam.
-   The [tidyquant](https://cran.r-project.org/package=tidyquant) package re-arranges functionality from several other key packages for use in the so-called tidyverse.
-   The [BCC1997](https://cran.r-project.org/package=BCC1997) prices European options under the Bakshi, Cao anc Chen (1997) model for stochastic volatility, stochastuc rates and random jumps.
-   The [Sim.DiffProc](https://cran.r-project.org/package=Sim.DiffProc) package provides functions to simulate and analyse multidimensional Itô and Stratonovitch stochastic calculus for continuous-time models.

**Risk management**

-   The Task View [ExtremeValue](https://cran.r-project.org/web/views/ExtremeValue.html) regroups a number of relevant packages.
-   The packages [CreditMetrics](https://cran.r-project.org/package=CreditMetrics/index.html) and [crp.CSFP](../packages/crp.CSFP) provide function for modelling credit risks.
-   The [mvtnorm](https://cran.r-project.org/package=mvtnorm) package provides code for multivariate Normal and t-distributions.
-   The Rmetrics packages [fPortfolio](https://cran.r-project.org/package=fPortfolio/index.html) and [fExtremes](../packages/fExtremes) also contain a number of relevant functions.
-   The [copula](https://cran.r-project.org/package=copula/index.html) and [fgac](../packages/fgac) packages cover multivariate dependency structures using copula methods.
-   The [actuar](https://cran.r-project.org/package=actuar) package provides an actuarial perspective to risk management.
-   The [ghyp](https://cran.r-project.org/package=ghyp) package provides generalized hyberbolic distribution functions as well as procedures for VaR, CVaR or target-return portfolio optimizations.
-   The [ChainLadder](https://cran.r-project.org/package=ChainLadder/index.html) package provides functions for modeling insurance claim reserves; and the [lifecontingencies](../packages/lifecontingencies) package provides functions for financial and actuarial evaluations of life contingencies.
-   The [frmqa](https://cran.r-project.org/package=frmqa) package aims to collect functions for Financial Risk Management and Quantitative Analysis.
-   The [ESG](https://cran.r-project.org/package=ESG) package can be used to model for asset projection, a scenario-based simulation approach.
-   The [riskSimul](https://cran.r-project.org/package=riskSimul) package provides efficient simulation procedures to estimate tail loss probabilities and conditional excess for a stock portfolios where log-returns are assumed to follow a t-copula model with generalized hyperbolic or t marginals.
-   The [GCPM](https://cran.r-project.org/package=GCPM) package anlyzes the default risk of credit portfolio using both analytical and simulation approaches.
-   The [FatTailsR](https://cran.r-project.org/package=FatTailsR) package provides a family of four distributions tailored to distribution with symmetric and asymmetric fat tails.
-   The [Dowd](https://cran.r-project.org/package=Dowd) package contains functions ported from the 'MMR2' toolbox offered in Kevin Dowd's book "Measuring Market Risk".
-   The [PortRisk](https://cran.r-project.org/package=PortRisk) package computes portfolio risk attribution.
-   The [NetworkRiskMeasures](https://cran.r-project.org/package=NetworkRiskMeasures) package implements some risk measures for financial networks such as DebtRank, Impact Susceptibility, Impact Diffusion and Impact Fluidity.

**Books**

-   The [FinTS](https://cran.r-project.org/package=FinTS) package provides an R companion to Tsay (2005), *Analysis of Financial Time Series* , 2nd ed. Wiley, and includes data sets, functions and script files to work some of the examples.
-   The [NMOF](https://cran.r-project.org/package=NMOF) package provides functions, examples and data from *Numerical Methods and Optimization in Finance* by Manfred Gilli, Dietmar Maringer and Enrico Schumann (2011), including the different optimization heuristics such as Differential Evolution, Genetic Algorithms, Particle Swarms, and Threshold Accepting.
-   The [FRAPO](https://cran.r-project.org/package=FRAPO) package provides data sets and code for the book *Financial Risk Modelling and Portfolio Optimization with R* by Bernhard Pfaff (2013).

**Data and date management**

-   The [zoo](https://cran.r-project.org/package=zoo/index.html) and [timeDate](../packages/timeDate/index.html) (part of Rmetrics) packages provide support for irregularly-spaced time series. The [xts](../packages/xts/index.html) package extends [zoo](../packages/zoo) specifically for financial time series. See the [TimeSeries](https://cran.r-project.org/web/views/TimeSeries.html) task view for more details.
-   [timeDate](https://cran.r-project.org/package=timeDate) also addresses calendar issues such as recurring holidays for a large number of financial centers, and provides code for high-frequency data sets.
-   The [fame](https://cran.r-project.org/package=fame/index.html) package can access Fame time series databases (but also requires a Fame backend). The [tis](../packages/tis) package provides time indices and time-indexed series compatible with Fame frequencies.
-   The [TSdbi](https://cran.r-project.org/package=TSdbi) package provides a unifying interface for several time series data base backends, and its SQL implementations provide a database table design.
-   The [IBrokers](https://cran.r-project.org/package=IBrokers) package provides access to the Interactive Brokers API for data access (but requires an account to access the service).
-   The [data.table](https://cran.r-project.org/package=data.table) package provides very efficient and fast access to in-memory data sets such as asset prices.
-   The [TFX](https://cran.r-project.org/package=TFX) package provides an interface to the TrueFX (TM) service for free streaming real-time and historical tick-by-tick market data for interbank foreign exchange rates at the millisecond resolution.
-   The package [highfrequency](https://cran.r-project.org/package=highfrequency) contains functionality to manage, clean and match highfrequency trades and quotes data and enables users to calculate various liquidity measures, estimate and forecast volatility, and investigate microstructure noise and intraday periodicity.
-   The [Rbitcoin](https://cran.r-project.org/package=Rbitcoin) package offers access to Bitcoin exchange APIs (mtgox, bitstamp, btce, kraken) via public and private API calls and integration of data structures for all markets.
-   The [bizdays](https://cran.r-project.org/package=bizdays) package compute business days if provided a list of holidays.
-   The [TAQMNGR](https://cran.r-project.org/package=TAQMNGR) package manages tick-by-tick (equity) transaction data performing 'cleaning', 'aggregation' and 'import' where cleaning and aggregation are performed according to Brownlees and Gallo (2006).
-   The [Rblpapi](https://cran.r-project.org/package=Rblpapi) package offers efficient access to the Bloomberg API and allows `bdp`, `bdh`, and `bds` queries as well as data retrieval both in (regular time-)bars and ticks (albeit without subsecond resolution).
-   The [finreportr](https://cran.r-project.org/package=finreportr/index.html) package can download reports from the SEC Edgar database, and relies on, inter alia, the [XBRL](../packages/XBRL) package for parsing these reports.
-   The [GetTDData](https://cran.r-project.org/package=GetTDData/index.html) package imports Brazilian government bonds data (such as LTN, NTN-B and LFT ) from the Tesouro Direto website. The [GetHFData](../packages/GetHFData) package downloads and aggregates tick-by-tick trade data for equity and derivatives markets in Brazil.
-   The [fmdates](https://cran.r-project.org/package=fmdates) package implements common date calculations according to the ISDA schedules, and can check for business in different locales.

### CRAN packages:

-   [actuar](https://cran.r-project.org/package=actuar)
-   [AmericanCallOpt](https://cran.r-project.org/package=AmericanCallOpt)
-   [backtest](https://cran.r-project.org/package=backtest)
-   [bayesGARCH](https://cran.r-project.org/package=bayesGARCH)
-   [BCC1997](https://cran.r-project.org/package=BCC1997)
-   [BenfordTests](https://cran.r-project.org/package=BenfordTests)
-   [betategarch](https://cran.r-project.org/package=betategarch)
-   [bizdays](https://cran.r-project.org/package=bizdays)
-   [bootTimeInference](https://cran.r-project.org/package=bootTimeInference)
-   [BurStFin](https://cran.r-project.org/package=BurStFin)
-   [BurStMisc](https://cran.r-project.org/package=BurStMisc)
-   [CADFtest](https://cran.r-project.org/package=CADFtest)
-   [car](https://cran.r-project.org/package=car)
-   [ccgarch](https://cran.r-project.org/package=ccgarch)
-   [ChainLadder](https://cran.r-project.org/package=ChainLadder)
-   [copula](https://cran.r-project.org/package=copula)
-   [covmat](https://cran.r-project.org/package=covmat)
-   [CreditMetrics](https://cran.r-project.org/package=CreditMetrics)
-   [credule](https://cran.r-project.org/package=credule)
-   [crp.CSFP](https://cran.r-project.org/package=crp.CSFP)
-   [data.table](https://cran.r-project.org/package=data.table)
-   [derivmkts](https://cran.r-project.org/package=derivmkts)
-   [dlm](https://cran.r-project.org/package=dlm)
-   [Dowd](https://cran.r-project.org/package=Dowd)
-   [dse](https://cran.r-project.org/package=dse)
-   [dyn](https://cran.r-project.org/package=dyn)
-   [dynlm](https://cran.r-project.org/package=dynlm)
-   [egcm](https://cran.r-project.org/package=egcm)
-   [ESG](https://cran.r-project.org/package=ESG)
-   [factorstochvol](https://cran.r-project.org/package=factorstochvol)
-   [fame](https://cran.r-project.org/package=fame)
-   [fArma](https://cran.r-project.org/package=fArma) (core)
-   [fAsianOptions](https://cran.r-project.org/package=fAsianOptions) (core)
-   [fAssets](https://cran.r-project.org/package=fAssets) (core)
-   [FatTailsR](https://cran.r-project.org/package=FatTailsR)
-   [fBasics](https://cran.r-project.org/package=fBasics) (core)
-   [fBonds](https://cran.r-project.org/package=fBonds) (core)
-   [fCopulae](https://cran.r-project.org/package=fCopulae) (core)
-   [fExoticOptions](https://cran.r-project.org/package=fExoticOptions) (core)
-   [fExtremes](https://cran.r-project.org/package=fExtremes) (core)
-   [fgac](https://cran.r-project.org/package=fgac)
-   [fGarch](https://cran.r-project.org/package=fGarch) (core)
-   [fImport](https://cran.r-project.org/package=fImport) (core)
-   [financial](https://cran.r-project.org/package=financial)
-   [FinancialMath](https://cran.r-project.org/package=FinancialMath)
-   [FinAsym](https://cran.r-project.org/package=FinAsym)
-   [finreportr](https://cran.r-project.org/package=finreportr)
-   [FinTS](https://cran.r-project.org/package=FinTS)
-   [fmdates](https://cran.r-project.org/package=fmdates)
-   [fMultivar](https://cran.r-project.org/package=fMultivar) (core)
-   [fNonlinear](https://cran.r-project.org/package=fNonlinear) (core)
-   [fOptions](https://cran.r-project.org/package=fOptions) (core)
-   [forecast](https://cran.r-project.org/package=forecast)
-   [fPortfolio](https://cran.r-project.org/package=fPortfolio) (core)
-   [fracdiff](https://cran.r-project.org/package=fracdiff)
-   [fractal](https://cran.r-project.org/package=fractal)
-   [FRAPO](https://cran.r-project.org/package=FRAPO)
-   [fRegression](https://cran.r-project.org/package=fRegression) (core)
-   [frmqa](https://cran.r-project.org/package=frmqa)
-   [fTrading](https://cran.r-project.org/package=fTrading) (core)
-   [fUnitRoots](https://cran.r-project.org/package=fUnitRoots) (core)
-   [GCPM](https://cran.r-project.org/package=GCPM)
-   [GetHFData](https://cran.r-project.org/package=GetHFData)
-   [gets](https://cran.r-project.org/package=gets)
-   [GetTDData](https://cran.r-project.org/package=GetTDData)
-   [GEVStableGarch](https://cran.r-project.org/package=GEVStableGarch)
-   [ghyp](https://cran.r-project.org/package=ghyp)
-   [gmm](https://cran.r-project.org/package=gmm)
-   [gogarch](https://cran.r-project.org/package=gogarch)
-   [GUIDE](https://cran.r-project.org/package=GUIDE)
-   [highfrequency](https://cran.r-project.org/package=highfrequency)
-   [IBrokers](https://cran.r-project.org/package=IBrokers)
-   [InfoTrad](https://cran.r-project.org/package=InfoTrad)
-   [lgarch](https://cran.r-project.org/package=lgarch)
-   [lifecontingencies](https://cran.r-project.org/package=lifecontingencies)
-   [lmtest](https://cran.r-project.org/package=lmtest)
-   [longmemo](https://cran.r-project.org/package=longmemo)
-   [LSMonteCarlo](https://cran.r-project.org/package=LSMonteCarlo)
-   [maRketSim](https://cran.r-project.org/package=maRketSim)
-   [markovchain](https://cran.r-project.org/package=markovchain)
-   [MarkowitzR](https://cran.r-project.org/package=MarkowitzR)
-   [matchingMarkets](https://cran.r-project.org/package=matchingMarkets)
-   [MSBVAR](https://cran.r-project.org/package=MSBVAR)
-   [MSGARCH](https://cran.r-project.org/package=MSGARCH)
-   [mvtnorm](https://cran.r-project.org/package=mvtnorm)
-   [NetworkRiskMeasures](https://cran.r-project.org/package=NetworkRiskMeasures)
-   [nlme](https://cran.r-project.org/package=nlme)
-   [NMOF](https://cran.r-project.org/package=NMOF)
-   [obAnalytics](https://cran.r-project.org/package=obAnalytics)
-   [opefimor](https://cran.r-project.org/package=opefimor)
-   [OptHedging](https://cran.r-project.org/package=OptHedging)
-   [OptionPricing](https://cran.r-project.org/package=OptionPricing)
-   [pa](https://cran.r-project.org/package=pa)
-   [parma](https://cran.r-project.org/package=parma)
-   [pbo](https://cran.r-project.org/package=pbo)
-   [PerformanceAnalytics](https://cran.r-project.org/package=PerformanceAnalytics) (core)
-   [pinbasic](https://cran.r-project.org/package=pinbasic)
-   [portfolio](https://cran.r-project.org/package=portfolio)
-   [PortfolioEffectHFT](https://cran.r-project.org/package=PortfolioEffectHFT)
-   [portfolioSim](https://cran.r-project.org/package=portfolioSim)
-   [PortRisk](https://cran.r-project.org/package=PortRisk)
-   [quantmod](https://cran.r-project.org/package=quantmod)
-   [QuantTools](https://cran.r-project.org/package=QuantTools)
-   [ragtop](https://cran.r-project.org/package=ragtop)
-   [Rbitcoin](https://cran.r-project.org/package=Rbitcoin)
-   [Rblpapi](https://cran.r-project.org/package=Rblpapi)
-   [Rcmdr](https://cran.r-project.org/package=Rcmdr)
-   [restimizeapi](https://cran.r-project.org/package=restimizeapi)
-   [riskSimul](https://cran.r-project.org/package=riskSimul)
-   [rmgarch](https://cran.r-project.org/package=rmgarch)
-   [RND](https://cran.r-project.org/package=RND)
-   [RQuantLib](https://cran.r-project.org/package=RQuantLib)
-   [rugarch](https://cran.r-project.org/package=rugarch) (core)
-   [rwt](https://cran.r-project.org/package=rwt)
-   [sandwich](https://cran.r-project.org/package=sandwich)
-   [sde](https://cran.r-project.org/package=sde)
-   [SharpeR](https://cran.r-project.org/package=SharpeR)
-   [sharpeRratio](https://cran.r-project.org/package=sharpeRratio)
-   [Sim.DiffProc](https://cran.r-project.org/package=Sim.DiffProc)
-   [SmithWilsonYieldCurve](https://cran.r-project.org/package=SmithWilsonYieldCurve)
-   [stochvol](https://cran.r-project.org/package=stochvol)
-   [stockPortfolio](https://cran.r-project.org/package=stockPortfolio)
-   [strucchange](https://cran.r-project.org/package=strucchange)
-   [TAQMNGR](https://cran.r-project.org/package=TAQMNGR)
-   [tawny](https://cran.r-project.org/package=tawny)
-   [termstrc](https://cran.r-project.org/package=termstrc)
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
-   [tsfa](https://cran.r-project.org/package=tsfa)
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
-   [Zelig](https://cran.r-project.org/package=Zelig)
-   [zoo](https://cran.r-project.org/package=zoo) (core)

### Related links:

-   CRAN Task View: [Econometrics](Econometrics.html)
-   CRAN Task View: [ExtremeValue](ExtremeValue.html)
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
