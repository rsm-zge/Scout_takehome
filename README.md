
# Scout Take-Home Assessment

This folder contains my submission for the Scout take-home assessment.

## Business Question

Which products should Scout prioritize for personalized recommendations and price-drop alerts?

## Files

- `decision_memo.pdf`One-page decision memo written for a fictional Head of Product at Scout.
- `scout_analysis.ipynb`Supporting Jupyter Notebook with data cleaning, product-level analysis, recommendation scoring, and visualizations.
- `Online Retail.xlsx`
  Source dataset used for the analysis.

## Dataset

The analysis uses the UCI Online Retail Dataset, a public transaction-level dataset from a UK-based online retailer. The dataset includes invoice number, product code, product description, quantity, invoice date, unit price, customer ID, and country.

Dataset source: UCI Machine Learning Repository, Online Retail Dataset. [www.kaggle.com/datasets/jihyeseo/online-retail-data-set-from-uci-ml-repo](https://www.kaggle.com/datasets/jihyeseo/online-retail-data-set-from-uci-ml-repo)

## Analysis Summary

The notebook focuses on product-level prioritization. I removed cancelled invoices, invalid transaction values, and non-product records such as postage, bank charges, Amazon fees, manual adjustments, and bad debt adjustments.

I then separated product opportunities into two tracks:

1. **Personalized recommendations**Products with strong revenue, order count, and quantity sold.
2. **Price-drop alerts**
   Higher-ticket products with enough order history to suggest real demand.

## How to Run

Open `scout_analysis.ipynb` in Jupyter Notebook or Google Colab and run the cells from top to bottom.

Required Python packages:

```python
pandas
numpy
matplotlib
openpyxl
```
