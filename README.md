# Integrated Retail Analytics for Store Optimization and Demand Forecasting

This project analyzes weekly retail sales to identify unusual patterns,
segment stores, explore department sales associations, and forecast sales.

## Project Components
- Data cleaning and exploratory analysis
- Sales anomaly detection
- Store segmentation and evaluation
- Department association analysis
- One-week and thirteen-week sales forecasting
- External-factor analysis
- Inventory and marketing recommendations

## Tools
Python, pandas, NumPy, Matplotlib, scikit-learn, and Google Colab.

## Repository Structure

- [Jupyter Notebook](Retail_Analytics.ipynb)
- [Python Code](retail_analytics.py)
- [Datasets](data/)
- [Charts and Analysis Results](outputs/)
- [Detailed Project Report](reports/)

## Key Findings

### One-Week Sales Forecasting
The selected core gradient boosting model achieved:
- MAE: 1,276.44
- RMSE: 2,652.42
- WAPE: 8.06%

Results were measured on 38,009 common test observations.
MAE was approximately 16.3% lower than the last-week baseline.

Adding lagged external features increased validation MAE by
2.93% under the tested settings.

### Thirteen-Week Sales Forecasting
The seasonal baseline achieved the lowest validation MAE
of 2,017.54 and was selected. The direct boosting model had
a lower RMSE, but MAE was the selection criterion.

### Store Segmentation
K-Means identified two store segments containing 35 and
10 stores, with a silhouette score of approximately 0.457.

## Interpretation and Limitations

- Segments describe stores, not individual customers.
- Department associations are exploratory sales-pattern
  relationships, not evidence of products purchased together.
- Forecasts predict sales amounts, not product quantities.
- Anomaly flags identify records for investigation;
  they do not prove data errors.
- Forecast evaluation uses chronological splits.
- Historical forecasting results do not establish current
  retail demand or causal effects of promotions.

## Running the Notebook

1. Open Retail_Analytics.ipynb in Google Colab.
2. Place the three CSV datasets in your project data folder.
3. Adjust the notebook's project path to your Drive location.
4. Run cells from top to bottom, including Drive mounting.
5. Review the generated charts, metrics, and saved outputs.


## Project Links

- [Open Notebook in Google Colab](https://colab.research.google.com/drive/1sLJRpTlJrTHuM1aEALE04hKD6J5_KcmL?usp=sharing)
- [Read Detailed Project Report](https://docs.google.com/document/d/1DpD94rVaBdYI1wBZ_6hVlDMx491OFwn1HPQlISVvooY/edit?usp=sharing)
## Author
Dolly Jain
