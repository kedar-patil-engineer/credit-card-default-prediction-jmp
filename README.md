# Predicting Credit Card Default using JMP Pro

A data mining study that predicts credit card payment defaulters using six models in
JMP Pro, comparing their performance to recommend the best classifier for credit risk
assessment.

> **Note on dates:** This project was originally completed in December 2019 as a
> BAN 620 Data Mining group project during my MS in Business Analytics at California
> State University, East Bay. It was uploaded to GitHub in June 2026 after my previous
> GitHub account was deleted. Commit dates are set to reflect the original completion
> date.

## Overview

Credit risk assessment is pivotal for financial institutions seeking to avoid financial
loss and reduce the number of defaulters. Credit risk is the risk of default on a credit
card payment arising from a customer failing to make required payments. The goal of this
project is to predict whether a customer will pay their debt on time next month, and to
decide on a cut-off criterion for classifying defaulters and non-defaulters.

### Goals

- Predict credit card payment defaulters and non-defaulters for the next month
- Build a data mining model that determines defaulters with high accuracy
- Identify reliable customers who can make payments on time
- Classify potential defaulters according to profiling and propensity

## Dataset

- **Source:** Default of Credit Card Clients (Taiwanese financial firm)
- **Period:** April 2005 to September 2005
- **Size:** 30,000 unique customers, 25 variables
- **Target:** `default.payment.next.month`
- **Class balance:** 6,636 defaulters vs 23,364 non-defaulters (about 22% / 78%)

## Models Built

| # | Model |
|---|-------|
| 1 | Decision Tree |
| 2 | Boosted Tree |
| 3 | K-Nearest Neighbor |
| 4 | Fit Nominal Logistic |
| 5 | Neural Network |
| 6 | Bootstrap Forest |

Models were compared on misclassification rate, RMSE, R square, and overfitting, then
tuned to better control type 2 errors.

## Result

The **Bootstrap Forest** marginally outperformed the other models and, after tuning,
classified type 2 errors more efficiently with an overall accuracy of about **71%**.
The conclusion is that Taiwanese financial institutions can use the Bootstrap Forest
model to reduce credit risk and safeguard against potential losses.

## Tech Stack

JMP Pro (SAS), statistical data mining and predictive modeling.

## Files

- `Data Mining Report .pdf` - full 20 page project report
- `Project_F.jmp` - JMP project data and models
- `Project Overview.docx` - project summary

## License

This project is released under the MIT License. See [LICENSE](LICENSE).

## Author

Kedar Patil - MS Business Analytics, California State University, East Bay
(group project)
