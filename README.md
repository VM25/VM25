<div align="center">

# Vatsal Maniar

### Quantitative Finance · Derivatives & Rates Risk · Systematic Research · Python Research Systems

M.S. Financial Engineering @ Stevens Institute of Technology · B.S. Computer Science (Magna Cum Laude) @ Arizona State · Jersey City, NJ

[![Portfolio](https://img.shields.io/badge/Portfolio-0B1F3A?style=for-the-badge&logo=netlify&logoColor=white)](https://maniar-portfolio.netlify.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vatsal-maniar)
[![Email](https://img.shields.io/badge/Email-1A1A1A?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vatsalmaniar2003@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/VM25)

**Markets · Risk · Research Engineering · Financial Data Systems**

I build quant systems that turn market data, pricing models, and research hypotheses into **validated, explainable decisions** — across derivatives, rates, portfolios, and credit.

</div>

---

## 🧠 Executive Snapshot

A Financial Engineering graduate student with a Computer Science core, building production-style quant and risk systems rather than one-off notebooks. My work spans **derivatives pricing, rates and curve risk, portfolio construction, systematic signal research, and credit/fraud decisioning** — each project taken from raw market data through a reproducible Python pipeline to a measured, explainable result.

I'm equally comfortable engineering the research engine and building the interface that makes it readable. The throughline is discipline: every number is priced offline from public data, stress-tested, and attributed to its drivers before it's reported.

---

## 📊 Selected Quant & Risk Systems

### Systematic Alpha Research Lab
> **Does a signal survive reality?** Tests whether cross-asset systematic signals endure realistic costs, out-of-sample decay, regime shifts, and market stress across two decades of data.

`walk-forward validation` · `cost-aware backtesting` · `regime stress` · `out-of-sample decay`

**Methods** — Expanding-window walk-forward (2006 → present) over 15 liquid ETFs; 5 bps/turnover cost model; crisis-window stress (GFC '08, Euro '11, COVID '20, Rates '22); parameter-robustness and rebalance-frequency sensitivity. Outcome: 3 signals survived, 1 conditional, 1 rejected.
**Proves** — Research discipline and the judgment to *reject* signals that don't clear costs and out-of-sample testing — not just to report the ones that look good.

**[Live report ↗](https://alpha-research.netlify.app)** · [Repository](https://github.com/VM25/research-lab)

<br>

### FX Options Risk Lab
> A **USD/MXN options book** analyzed end to end — pricing, Greeks, hedging, tail risk, and P&L attribution.

`Garman–Kohlhagen` · `Greeks` · `VaR / ES` · `Monte Carlo` · `P&L attribution`

**Methods** — Garman–Kohlhagen pricing; delta/gamma/vega/theta; static spot hedge with residual gamma/vega exposure; 1-day 95% / 99% VaR and Expected Shortfall via 10,000-path Monte Carlo; joint spot–vol stress repricing; full P&L decomposed into Greek channels plus residual.
**Proves** — Derivatives pricing and the ability to take a hedged book apart into the risks that actually drive its P&L.

**[Live demo ↗](https://fxrisklab.netlify.app)** · [Repository](https://github.com/VM25/fx-options-risk-lab)

<br>

### Inflation Regime Rates Risk Engine
> How an inflation regime breaks the textbook long-duration Treasury hedge — repriced **cash flow by cash flow** under a shocked curve.

`key-rate DV01` · `convexity` · `real-rate / breakeven attribution` · `Vasicek / CIR`

**Methods** — Regime curve shocks (incl. a measured 2022 replay); modified duration, total and key-rate DV01; exact vs duration-only vs convexity-adjusted repricing; a channel waterfall splitting P&L into duration, real-rate, breakeven, convexity and curve-shape; rule-based hedge overlays; Vasicek/CIR short-rate simulation (10,000 paths) with 1-year VaR/ES.
**Proves** — Rates and curve analytics, and the macro-risk decomposition that explains *why* a "safe" hedge fails.

**[Live demo ↗](https://yieldshock.netlify.app)** · [Repository](https://github.com/VM25/inflation-lab)

<br>

### Portfolio Risk & Allocation Analytics
> *Four allocation rules, three crisis windows, eighteen years of regime change* — across a 13-ETF multi-asset universe.

`Equal Weight / GMV / Max Sharpe` · `regime-aware` · `drawdowns` · `correlation regimes` · `turnover`

**Methods** — Equal Weight, Global Minimum Variance, Max Sharpe, and a rules-based Regime-Aware allocator; maximum-drawdown paths; 95% VaR/CVaR; monthly turnover and cumulative cost drag; correlation matrices under normal vs. defensive regimes; effective independent bets.
**Proves** — Portfolio construction with a clear-eyed view of correlation instability, crisis behavior, and the gap between in-sample optimality and real-world turnover.

**[Live demo ↗](https://pra-analytics.netlify.app)** · [Repository](https://github.com/VM25/portfolio-lab)

<br>

### Credit & Payments Risk Decision Engine
> Translates borrower, account, and transaction signals into **underwriting decisions** — scores, expected loss, fraud controls, and policy tradeoffs.

`expected loss` · `policy thresholds` · `fraud controls` · `model-risk validation` · `scikit-learn`

**Methods** — Risk scoring and expected-loss estimation; policy-threshold tradeoffs mapped to approve / manual-review / decline decisions; fraud and payments controls; model-risk validation evidence — built on a scikit-learn / pandas pipeline.
**Proves** — Credit and fraud/payments decisioning as a system: not just a model score, but the policy and validation layer that turns a score into a defensible decision.

**[Live demo ↗](https://credits-engine.netlify.app)** · [Repository](https://github.com/VM25/credits-lab)

<br>

### ApexGP Markets — Event-Market Microstructure
> Treats the official **2025 Formula 1 season** as tradable binary event-markets — a sandbox for probability repricing, microstructure, and portfolio risk.

`event markets` · `binary contracts` · `mark-to-market` · `microstructure` · `settlement`

**Methods** — Real-season replay turning race telemetry into binary contracts; a $100k sandbox book with mark-to-market portfolio analytics; probability repricing, market-microstructure mechanics, settlement logic, and championship-futures tracking.
**Proves** — How information becomes price — event-driven trading mechanics and live portfolio risk in a self-contained market environment.

**[Live demo ↗](https://apexgp-markets.netlify.app)** · [Repository](https://github.com/VM25/apexgp-markets)

---

## 🛠️ Technical Stack

**Research & Modeling** — Python · NumPy · SciPy · pandas · scikit-learn · QuantLib
**Quant & Risk** — Garman–Kohlhagen pricing · Greeks · VaR / ES · key-rate DV01 · Vasicek / CIR · portfolio optimization (GMV / Max Sharpe) · walk-forward backtesting · stress testing · expected-loss & scoring
**Data** — Yahoo Finance · FRED · NBER · Cboe · Kenneth French Data Library · reproducible offline pipelines (CSV/JSON research outputs)
**Interfaces** — TypeScript · React · Next.js · Tailwind CSS · Recharts
**Also** — C++ · R · MATLAB · Bloomberg & LSEG (market-data exposure)
**Workflow** — Git / GitHub · Netlify · reproducible, offline research pipelines

---

## 🔬 What I Build

Research engines, not toy notebooks. Decision systems, not static dashboards.

> The hard part is never computing a Sharpe ratio, a VaR number, or a credit score — it's proving the number deserves to be trusted.

- **Validation-first.** Every result survives transaction costs, out-of-sample windows, and stress before it's reported. Signals that don't clear the bar get rejected, on the record.
- **Explainable by construction.** Models expose their assumptions; P&L is attributed to its drivers; a shock can be read link by link from cause to consequence.
- **Reproducible.** Numbers are generated offline by Python pipelines from public data — nothing is priced in the browser, and there are no black boxes.
- **Readable.** Each engine ships with an interface that makes the research legible to someone who didn't write it.

---

## 🧭 Currently

- **FRM Part I** — sitting August 2026
- **Quant research & risk-analytics recruiting** — full-time, 2026
- Systematic strategy validation; derivatives, rates, and portfolio risk systems
- Credit, fraud, and payments risk decisioning

---

## 🌐 Connect

[![Portfolio](https://img.shields.io/badge/Portfolio-0B1F3A?style=for-the-badge&logo=netlify&logoColor=white)](https://maniar-portfolio.netlify.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vatsal-maniar)
[![Email](https://img.shields.io/badge/Email-1A1A1A?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vatsalmaniar2003@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/VM25)

<div align="center"><sub>Full project portfolio and write-ups → <a href="https://maniar-portfolio.netlify.app">maniar-portfolio.netlify.app</a></sub></div>

