# Luke Freyman

Risk and fraud analytics. M.S. FinTech at UCF, graduating December 2027.
Open to 2027 analyst internships in fraud, credit risk, model risk and data.

Lake Mary, Florida · [LinkedIn](https://linkedin.com/in/luke-freyman-a22ab7249)

## Projects

Every number in the table below is produced by the code in that repo. None of it is typed in by hand.

| Project | What it does | Result |
|---|---|---|
| [fraud-detection-pipeline](https://github.com/lukefreyman-ai/fraud-detection-pipeline) | Card fraud model. The alert threshold is set from what a false alarm and a missed fraud each cost. | Catches 81% of fraud at 27 alerts per 10,000 transactions. Expected cost $3,166 against $3,457 for the next best model. |
| [aml-transaction-monitoring](https://github.com/lukefreyman-ai/aml-transaction-monitoring) | Eight SQL rules over 518,492 transactions, tuned to how many alerts an analyst can actually clear. | Precision 53% to 83%. 39 alerts a month instead of 58, with all 190 suspicious customers still caught. |
| [model-risk-monitoring](https://github.com/lukefreyman-ai/model-risk-monitoring) | Watches a deployed credit scorecard for drift and writes the validation report. | Flagged red: the score distribution moved past the 0.25 limit. Ranking power held at 0.72 Gini. |
| [credit-risk-scorecard](https://github.com/lukefreyman-ai/credit-risk-scorecard) | Seven-variable scorecard a lender could explain to a declined applicant. | AUC 0.857, Gini 0.713. Default rate runs from 54.2% in the lowest score band to 0.46% in the highest. |
| [medicare-claims-denial-analysis](https://github.com/lukefreyman-ai/medicare-claims-denial-analysis) | Runs CMS billing edits across 780,000 Medicare outpatient claims. | 4.1% of claims break a hard edit, roughly $1.22M at risk. 41% of that traces to a single code pair. |
| [complaint-triage](https://github.com/lukefreyman-ai/complaint-triage) | Measures how accurately an LLM sorts real CFPB complaints into nine categories. | 76.5% on a balanced set where guessing the largest class gets 11%. A prompt I expected to help scored 2.8 points worse, and that is in the README. |
| [tsmom-etf](https://github.com/lukefreyman-ai/tsmom-etf) | Momentum strategy on 10 ETFs, 2005 to 2026, with a paper-trading executor. | Sharpe 0.78 against 0.64 for SPY. Worst drawdown -11.6% against -55.2%. It does not beat SPY on return, and the README says so. |

## How these are built

- Thresholds come from a cost or an analyst budget, not from maximising a metric.
- Results that went the wrong way stay in the README.
- Results files are committed, so every number in a README traces back to the run that produced it.

## Now

A pipeline that reads every SEC Form 13F filing from 2010 to 2014 and reports institutional
ownership per company. 30 million holdings rows parsed. The 2013 Q4 output matches the SEC's
own data set on all 1,584,855 rows. The repo is private while the research is in progress,
and I can share it on request.
