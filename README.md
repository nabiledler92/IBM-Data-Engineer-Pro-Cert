# IBM-Data-Engineer-Pro-Cert

My ETL peer-review assignment from the **IBM Data Engineering Professional Certificate**: extract bank market-cap data, convert it from US dollars to British pounds, and load it to CSV with Python and pandas.

## Notebook

[`ETL_Engineer_Peer_Review_Assignment.ipynb`](ETL_Engineer_Peer_Review_Assignment.ipynb)

## The ETL steps

1. **Extract**: read `bank_market_cap_1.json` into a DataFrame with the columns `Name` and `Market Cap (US$ Billion)`.
2. **Transform**: look up the GBP rate in `exchange_rates.csv`, then convert each bank's market cap to GBP billions, rounded to 3 decimal places.
3. **Load**: write the result to `bank_market_cap_gbp.csv` without the index.
4. **Log**: write a timestamped entry to a log file at the start and end of each phase.

## Run it

Open the notebook in Jupyter or the IBM Skills Network lab. You need Python 3 with `pandas`. The notebook downloads its course datasets with `wget`.

## Tools

Python · pandas · glob · Jupyter

The assignment template and datasets come from IBM Skills Network course material.
