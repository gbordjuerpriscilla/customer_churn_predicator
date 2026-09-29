# Customer Churn Predictor



## What it does
- Flags customers who show 2 churn signals: prolonged inactivity (relative to their own ordering pattern) and a sharp drop in order frequency
- Ranks flagged customers by a 0–100 risk score
- Outputs a ranked list of at-risk customers (`at_risk_customers.csv`)

## Results
On the sample data (200 customers, 180 days), 70 customers (35%) were flagged. Of 35 customers deliberately made to look at-risk, 34 were caught. See the methodology note for the full write-up, including limitations.

## How it was built
Python (pandas) in Google Colab. See the notebook for the full analysis.

## Note on the data
The dataset is simulated, and some customers were deliberately made to look at-risk so the signals had something real to catch. It is not real customer data.

##What was hard
Trying use the two signals very efficiently. Making sure that customers are not flagged by mistake. 
