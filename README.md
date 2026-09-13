<div align="center">

# Vatsal Maniar

### Financial Engineering × Computer Science

**Pricing · Rates · Risk · Systematic Research · Decision Systems**

I build quantitative systems that turn market uncertainty into something you can **price, hedge, validate, and explain**.

M.S. Financial Engineering Candidate @ Stevens Institute of Technology  
B.S. Computer Science, *Magna Cum Laude* @ Arizona State University  
Jersey City, NJ · New York City Metro

[![Portfolio](https://img.shields.io/badge/Portfolio-0B1F3A?style=for-the-badge&logo=netlify&logoColor=white)](https://maniar-portfolio.netlify.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vatsal-maniar/)
[![Email](https://img.shields.io/badge/Email-8C744A?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vatsalmaniar2003@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/VM25)

**Markets · Risk · Research Engineering · Financial Data Systems**

</div>

---

## 🧠 Executive Snapshot

I work at the intersection of **quantitative finance, risk, and software engineering**—building production-style research and decision systems rather than one-off notebooks. My work spans derivatives pricing, Treasury curve risk, portfolio construction, systematic signal research, credit and fraud decisioning, and event-market microstructure.

Each system runs from raw data through a reproducible Python pipeline to tested research outputs and a deployed interface. I am equally comfortable engineering the model, validating the result, and building the software that makes it understandable.

---

## 📊 Selected Quant & Risk Systems

### Systematic Alpha Research Lab

> **Does a signal survive reality?** Five cross-asset strategies tested against costs, out-of-sample decay, parameter instability, regime shifts, and market stress.

`walk-forward validation` · `cost-aware backtesting` · `no look-ahead` · `regime stress`

**Methods** — Expanding-window research over 15 liquid ETFs from 2006 onward; signal-to-position lags; monthly rebalancing; cash fallback; 1/5/10/25 bps cost cases; train/test, walk-forward, parameter, and rebalance tests; stress windows spanning the GFC, Euro crisis, COVID shock, and 2022 rates selloff. Outcome: **3 signals survived, 1 was conditional, and 1 was rejected**.

**Proves** — Research discipline and the willingness to reject a strategy that fails costs or validation—not just report the backtests that look good.

**[Live research report ↗](https://alpha-research.netlify.app)** · [Repository](https://github.com/VM25/research-lab)

<br>

### FX Options Risk Lab

> A **USD/MXN options book** analyzed end to end—pricing, Greeks, hedging, tail risk, and P&L attribution.

`Garman–Kohlhagen` · `Greeks` · `VaR / ES` · `Monte Carlo` · `QuantLib validation`

**Methods** — Garman–Kohlhagen pricing; delta, gamma, vega, and theta; static spot hedging with residual gamma/vega exposure; 1-day 95% and 99% VaR/Expected Shortfall through 10,000-path joint spot-volatility Monte Carlo; full stress repricing; P&L decomposition into Greek channels plus residual; independent QuantLib benchmarking.

**Proves** — Derivatives pricing and the ability to take a hedged book apart into the risks that actually drive its P&L.

**[Live risk lab ↗](https://fxrisklab.netlify.app)** · [Repository](https://github.com/VM25/fx-options-risk-lab)

<br>

### Inflation Regime Rates Risk Engine

> How an inflation regime breaks the textbook long-duration Treasury hedge—repriced **cash flow by cash flow** under a shocked curve.

`DV01 / key-rate DV01` · `convexity` · `real-rate / breakeven attribution` · `Vasicek / CIR`

**Methods** — Ten curve-shock scenarios, including a measured 2022 replay; modified duration, total DV01, and key-rate DV01; exact versus duration-only and convexity-adjusted repricing; P&L attribution across real-rate, breakeven, duration, convexity, curve-shape, and residual channels; rule-based hedge overlays; 10,000-path Vasicek/CIR simulation with 1-year VaR/ES. The research pipeline closes with **40/40 validation checks passing**.

**Proves** — Rates and curve analytics, plus the macro-risk decomposition needed to explain *why* a supposedly safe hedge fails.

**[Live rates engine ↗](https://yieldshock.netlify.app)** · [Repository](https://github.com/VM25/inflation-lab)

<br>

### Portfolio Risk & Allocation Analytics

> *Four allocation rules, three crisis windows, and eighteen years of regime change* across a 13-ETF multi-asset universe.

`Equal Weight / GMV / Max Sharpe` · `regime-aware` · `drawdowns` · `factor exposure`

**Methods** — Equal Weight, Global Minimum Variance, Max Sharpe, and rules-based Regime-Aware allocation under common constraints; maximum-drawdown paths; 95% VaR/CVaR; turnover and cumulative cost drag; normal-versus-defensive correlation matrices; effective independent bets; Fama–French factor-exposure diagnostics.

**Proves** — Portfolio construction with a clear view of correlation instability, crisis behavior, and the gap between in-sample optimality and implementable allocation.

**[Live analytics ↗](https://pra-analytics.netlify.app)** · [Repository](https://github.com/VM25/portfolio-lab)

<br>

### Credit & Payments Risk Decision Engine

> Turns borrower, account, and transaction evidence into **underwriting decisions**—not merely model scores.

`expected loss` · `policy thresholds` · `fraud controls` · `model-risk validation`

**Methods** — Risk scoring and expected loss (`EL = PD × LGD × EAD`); approve / manual-review / decline thresholds; policy trade-off simulation; fraud and payments controls; portfolio monitoring; model-risk validation; transparent labeling of real and synthetic inputs across credit, card-transaction, stablecoin-flow, and macro data.

**Proves** — Credit and fraud decisioning as a complete system: evidence → model → policy → defensible action.

**[Live decision engine ↗](https://credits-engine.netlify.app)** · [Repository](https://github.com/VM25/credits-lab)

<br>

### ApexGP Markets — Event-Market Microstructure

> Treats the official **2025 Formula 1 season** as a portfolio of tradable binary event markets.

`event markets` · `binary contracts` · `mark-to-market` · `microstructure` · `settlement`

**Methods** — Real-season replay across 24 races and 500+ contracts; telemetry-driven probability repricing; circuit breakers; race settlement and championship futures; a $100,000 sandbox book with mark-to-market P&L, exposure limits, drawdown monitoring, Sharpe analytics, and a complete transaction audit.

**Proves** — How information becomes price: event-driven trading mechanics, market microstructure, and live portfolio risk inside a self-contained market environment.

**[Live market simulator ↗](https://apexgp-markets.netlify.app)** · [Repository](https://github.com/VM25/apexgp-markets)

---

## 🔬 What I Build

**Research engines, not toy notebooks. Decision systems, not static dashboards.**

> The hard part is not computing a Sharpe ratio, a VaR number, or a credit score—it is proving the number deserves to be trusted.

- **Validation first.** Results face transaction costs, out-of-sample windows, stress scenarios, and independent checks before they are reported.
- **Explainable by construction.** Assumptions stay visible; P&L is attributed to its drivers; policy decisions can be traced back to evidence.
- **Reproducible.** Python pipelines generate deterministic research artifacts from documented data sources—no opaque browser-side calculations or black boxes.
- **Engineered end to end.** Research code, tests, data contracts, frontend, documentation, and deployment are treated as one system.
- **Readable.** Every engine ships with an interface that makes the analysis legible to someone who did not build it.

---

## 🛠️ Technical Stack

**Research & Modeling** — Python · NumPy · SciPy · pandas · scikit-learn · QuantLib  
**Quant & Risk** — Garman–Kohlhagen · Greeks · Monte Carlo · VaR / ES · DV01 / KRD · Vasicek / CIR · portfolio optimization · walk-forward backtesting · stress testing · expected loss  
**Data** — Yahoo Finance · FRED · NBER · Cboe · Kenneth French Data Library · reproducible CSV/JSON pipelines  
**Interfaces** — TypeScript · React · Next.js · Tailwind CSS · Recharts  
**Also** — C++ · R · MATLAB · Bloomberg and LSEG market-data exposure  
**Workflow** — Git · GitHub · testing · Netlify · continuous deployment

---

## 🧭 Currently

- **FRM Part I Candidate** — August 2026
- Open to **Fall 2026 quant co-op / internship** opportunities
- Targeting **full-time 2027** roles across quantitative research, trading, derivatives, risk, and quantitative engineering
- Current research interests: systematic-strategy validation; derivatives, rates, and portfolio risk; credit, fraud, and payments decisioning

---

## 🌐 Connect

[![Portfolio](https://img.shields.io/badge/Portfolio-0B1F3A?style=for-the-badge&logo=netlify&logoColor=white)](https://maniar-portfolio.netlify.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vatsal-maniar/)
[![Email](https://img.shields.io/badge/Email-8C744A?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vatsalmaniar2003@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/VM25)

<div align="center"><sub>Full project portfolio and detailed write-ups → <a href="https://maniar-portfolio.netlify.app">maniar-portfolio.netlify.app</a></sub></div>
