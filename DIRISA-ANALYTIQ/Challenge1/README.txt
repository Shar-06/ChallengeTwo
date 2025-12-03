ANALYTIQ LOAN OFFER STRATEGY
=============================

OVERVIEW
--------
This MATLAB solution optimizes loan offers to telecom customers to maximize portfolio profit under a R1M budget constraint.

DATA PREPARATION
----------------
- Features: monthly_arpu, tenure, late payments, balance, contract type
- Engineered: payment_risk, balance_ratio, contract_bin
- Split: 80% training, 20% validation

MODEL
-----
- Algorithm: Logistic regression (GLM with binomial distribution)
- Calibration: Probabilities scaled by 0.30 (optimal from validation)
- Output: Default probability p_i for each customer

LOAN DECISION RULES
-------------------
1. Loan amount: L_i = min(2*monthly_arpu, 10000), minimum R100
2. Term: n_i = 6 or 12 months (whichever gives higher profit)
3. Offer only if expected profit > 0
4. Budget: R1,000,000 allocated by profit efficiency ranking

PROFIT CALCULATION
------------------
6-month: L_i*(0.10-0.025) - p_i*L_i*0.70 - 30
12-month: L_i*(0.20-0.05) - p_i*L_i*0.70 - 30

FILES
-----
- main.m: Complete solution script
- submission.csv: Output file with customer_id, p_i, L_i, n_i
- train.csv: Training data (provided)
- test.csv: Test data (provided)

RUN INSTRUCTIONS
----------------
1. Place train.csv and test.csv in same folder
2. Run main.m in MATLAB
3. Results saved to submission.csv
