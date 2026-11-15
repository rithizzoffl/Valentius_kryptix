# Global Financial Markets EDA

## Overview

This project explores historical financial market data using Python, Pandas, Matplotlib, and Seaborn. The analysis focuses on price and trading volume patterns across stock indices, commodities, currencies, and cryptocurrencies.

## Dataset

[Global Financial Markets Dataset (2010–Present)](https://www.kaggle.com/datasets/belbino/global-financial-markets-dataset-2010-present)

The dataset contains daily market records with fields including date, open, high, low, close, volume, symbol, asset name, asset type, and region. The CSV is not included in this repository. Download it from Kaggle and place it beside the notebook before running the analysis.

## Analysis

The notebook includes:

- Dataset structure, data types, memory usage, and row previews
- Missing-value and duplicate checks
- Numeric summary statistics and categorical value counts
- A missing-values review
- Visualisations of asset-type counts, closing-price distribution, price correlations, S&P 500 closing prices, median volume by asset type, and S&P 500 daily returns
- A summary of key findings and data limitations

## Key Findings

- The dataset contains 192,010 rows and 10 columns, spanning January 3, 2000 to November 13, 2026.
- No missing values or exact duplicate rows were found.
- Stock indices have the most records among the four asset types; cryptocurrencies have the fewest.
- Closing prices across the combined asset groups are strongly right-skewed.
- The price fields are strongly positively correlated overall.
- S&P 500 daily returns fluctuate around zero, with some periods showing larger daily movements.
- Two negative WTI crude oil prices occur on April 20–21, 2020; these were retained and noted as unusual observations.

## Files

- `global_markets_eda.ipynb` — notebook containing the analysis
- `README.md` — project description and dataset information

## Requirements

Install the libraries if they are not already available:

```bash
pip install pandas matplotlib seaborn jupyter
```

## Running the Notebook

1. Download the CSV from the Kaggle dataset page.
2. Place the CSV in the same folder as `global_markets_eda.ipynb`.
3. Update the filename in the notebook’s `pd.read_csv()` cell if needed.
4. Open the notebook in Jupyter and run the cells from top to bottom.

## Limitations

This is an exploratory analysis of historical data. The dataset combines assets with different price scales and volume conventions, so aggregate comparisons should be interpreted carefully. Correlation shows association and does not establish causation.
