# Business Case Analysis

---

## B1. Problem Formulation

### (a)

We want to predict **items_sold**.
Inputs are store details, promotion type, and time.
This is a **regression problem** because the output is a number.

---

### (b)

Items sold is better than revenue because revenue changes with price and discounts.
Items sold shows real customer demand.

This means we must choose a target that matches the business goal.

---

### (c)

Instead of one model for all stores, we can group stores and create separate models.
This is better because different stores behave differently.

---

## B2. Data and EDA Strategy

### (a)

Data is joined using store_id and date.

Final dataset:
One row = one store per month

Data is grouped monthly before using in model.

---

### (b)

We can check:

* Sales vs promotion → which works best
* Sales vs location → urban vs rural
* Monthly trend → seasonal changes
* Competition vs sales → effect of competition

This helps in better modelling.

---

### (c)

Most data has no promotion, so model may become biased.

To fix:

* Balance the data
* Give more importance to promotion data

---

## B3. Model Evaluation and Deployment

### (a)

Use time-based split (past for training, future for testing).

Random split is wrong because it mixes past and future.

Metrics:

* RMSE → shows error
* MAE → easy to understand

---

### (b)

Feature importance shows why model makes decisions.

Different months have different demand, so model gives different results.

---

### (c)

Steps:

* Save model
* Use new data every month
* Predict results

Monitor:

* Check errors
* Retrain if performance drops

---

# Conclusion

Machine learning helps choose the best promotion and improves sales.
