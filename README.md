# Ahmad Reza Motezakker, PhD

Data scientist and quantitative researcher based in Stockholm. PhD in Engineering Mechanics from KTH Royal Institute of Technology. I build models on real data and validate them properly before trusting them, across quantitative finance, credit risk, and applied machine learning.

[LinkedIn](https://www.linkedin.com/in/ahmadrezamotezakker) · [Personal site](https://armotezakker.github.io) · [Google Scholar](https://scholar.google.ca/citations?user=_4nQ2p8AAAAJ)

## Projects

**[systematic-strategy-research](https://github.com/armotezakker/systematic-strategy-research)**
Momentum and short-term reversal signals, backtested with proven look-ahead controls and realistic transaction costs, then tested for statistical significance with a block bootstrap after finding and fixing a real confound in an earlier version of the test. Honest result: neither signal shows a significant edge net of costs in this universe, which is itself the correct, credible finding.

**[credit-risk-serving-api](https://github.com/armotezakker/credit-risk-serving-api)**
A live FastAPI service for a credit risk model, with MLflow experiment tracking, SHAP-based explainability narrated by a local language model, and population-stability drift monitoring. Found and fixed a real reliability issue in the explanation layer, then rebuilt the architecture so the failure mode could not recur.

**[credit-scoring-ifrs9](https://github.com/armotezakker/credit-scoring-ifrs9)**
A probability-of-default model built on 1.35 million real loan outcomes, with time-based out-of-time validation, a calibration bug found and fixed with Platt scaling, and IFRS9 staging and expected credit loss with a threshold chosen through sensitivity analysis rather than picked arbitrarily.

**[quant-risk-models](https://github.com/armotezakker/quant-risk-models)**
Markowitz portfolio optimization, Black-Scholes option pricing, Value at Risk, and Merton-Vasicek structural credit risk, built on real market data and backtested against real outcomes.

**[esg-credit-risk-model](https://github.com/armotezakker/esg-credit-risk-model)**
Merton structural credit model on 352 S&P 500 firms testing whether ESG risk predicts default risk after controlling for leverage, size, and sector, finding a clean null validated through influence diagnostics and sub-score decomposition. A climate transition stress overlay showed the shock amplifies risk only in firms that were already highly leveraged, leaving strong balance sheets unaffected even under a severe shock.

**[seasonal-anomaly-detection](https://github.com/armotezakker/seasonal-anomaly-detection)**
Seasonal and trend-aware anomaly detection tested on six real series from the Numenta Anomaly Benchmark, with two candidate fixes tested as separate ablations rather than bundled. One fix took a broken detector from catching 1 of 5 real anomalies to 5 of 5. The other backfired for a measured reason. On 4 of 6 series, the original naive detector was still the best result, reported honestly rather than hidden.

**[ai-power-event-study](https://github.com/armotezakker/ai-power-event-study)**
A market model event study testing whether real, dated news about AI data center power demand caused significant stock reactions, with a safeguard that caught a real data contamination case on the first live run. Two individually significant results did not survive a Bonferroni correction for multiple testing, the honest, complete answer once accounted for.

**[airline-price-elasticity](https://github.com/armotezakker/airline-price-elasticity)**
Route-level price elasticity of demand on 30 years of real US airline fare data. Found and fixed a 30-year trend confound, then a new overfitting problem introduced by that fix, both proven with tests that fail on the old code and pass on the new. Final elasticities land in a literature-consistent range, concentrated in leisure travel markets as economic theory predicts.

**[bigquery-loan-analytics](https://github.com/armotezakker/bigquery-loan-analytics)**
Real BigQuery data warehouse analysis on 1.35 million loan records, cutting query cost by 83 percent through column selection, with a discovery about the query optimizer's behavior along the way and an honest, correctly interpreted comparison against DuckDB.
