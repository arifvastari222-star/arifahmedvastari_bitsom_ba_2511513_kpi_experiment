# Hypothesis Testing Notes

## Objective

Evaluate whether the new onboarding experience significantly improves the Paid Conversion Rate compared to the existing onboarding process.

## Hypotheses

### Null Hypothesis (H₀)

The new onboarding experience does not improve the Paid Conversion Rate.

### Alternative Hypothesis (H₁)

The new onboarding experience improves the Paid Conversion Rate.

## Test Used

Two-Proportion Z-Test

## Inputs

| Metric          | Control | Treatment |
| --------------- | ------- | --------- |
| Users           | 693     | 715       |
| Conversions     | 22      | 50        |
| Conversion Rate | 3.17%   | 6.99%     |

## Test Results

* Z-Score: 3.41
* P-Value: 0.0003
* Significance Level (α): 0.05

## Decision

Since the p-value (0.0003) is less than the significance level (0.05), the Null Hypothesis is rejected.

## Interpretation

The analysis provides strong statistical evidence that the new onboarding experience significantly improves the Paid Conversion Rate. The observed improvement is unlikely to be due to random chance.
