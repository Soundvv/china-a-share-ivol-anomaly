# Idiosyncratic Volatility Anomaly in China A Shares

This repository contains a cleaned notebook from a course group project examining the idiosyncratic-volatility anomaly in the Chinese A-share market. The analysis uses monthly observations from 2001 to 2010, forms IVOL-sorted portfolios, and evaluates abnormal returns under CAPM, Fama–French three-factor, and China-specific four-factor models.

## Highlights

- 100,687 monthly observations covering 1,662 A-share stocks.
- Monthly quintile portfolios formed using Fama–French three-factor idiosyncratic volatility.
- Equal-weighted low-minus-high IVOL return of 17.55% annualized.
- Sharpe ratio of 1.68 and maximum drawdown of -11.40%.
- CH-4 annualized alpha of 11.58% with a t-statistic of 3.18.

## Repository structure

```text
notebooks/
  ivol_anomaly_analysis.ipynb
results/
  key_results.csv
DATA.md
requirements.txt
```

## Running the notebook

Create a Python environment and install the dependencies:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

Place an authorized copy of the source dataset in the repository root as `csmar_0110sample.dta`, then open the notebook. The licensed dataset is intentionally excluded from this repository.

## Method summary

Stocks are sorted into five IVOL portfolios each month. The analysis reports equal- and value-weighted portfolio performance, constructs a low-minus-high IVOL portfolio, and estimates CAPM, Fama–French three-factor, and China-specific four-factor regressions.

## Research limitations

- The sample ends in 2010 and should not be interpreted as evidence of current implementable performance.
- Reported portfolio returns do not deduct transaction costs or market impact.
- The underlying CSMAR data are licensed and are not redistributed.
- Results are historical research estimates and are not investment advice.

## Project note

This work originated as a course group project. The repository is a cleaned research artifact for portfolio review and excludes documents containing group-member information.
