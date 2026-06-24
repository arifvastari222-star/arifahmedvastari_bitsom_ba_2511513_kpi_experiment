# A/B Testing KPI Framework Analysis and Business Recommendation

## 1. Business Context

A SaaS company conducted an A/B experiment to evaluate a redesigned onboarding experience. The objective was to determine whether the new onboarding flow could improve user activation, engagement, and conversion to paid subscriptions while maintaining a positive customer experience.

The experiment compared a Control group (existing onboarding experience) with a Treatment group (new onboarding experience).

---

## 2. Dataset Description

The dataset contains user-level experiment data including:

* User ID
* Experiment Group (Control/Treatment)
* Region
* Device Type
* Traffic Source
* Plan Type
* Landing Page Visit
* Trial Started
* Onboarding Completed
* Converted to Paid
* Revenue (30 Days)
* Support Tickets (30 Days)
* Refund Requested
* Days to Convert
* Engagement Score

The dataset was validated through data quality checks including missing values, duplicate records, binary field validation, outlier assessment, and segment distribution analysis.

---

## 3. North Star Metric Selected

### Paid Conversion Rate

Paid Conversion Rate was selected as the North Star Metric because it directly measures the percentage of users who become paying customers and aligns with the primary business objective of increasing revenue and customer acquisition.

Control Group: 3.17%

Treatment Group: 6.99%

Improvement: +3.82 percentage points

---

## 4. KPI Tree Summary

### North Star Metric

* Paid Conversion Rate

### Primary Drivers

* Landing Page Effectiveness
* Trial Activation
* User Monetization
* User Engagement

### Sub-Drivers

* Landing Page Visit Rate
* Traffic Source Quality
* Trial Start Rate
* Onboarding Completion Rate
* Average Revenue Per User (ARPU)
* Average Revenue Per Converted User
* Engagement Score
* Days to Convert

### Guardrail Metrics

* Refund Rate
* Support Ticket Rate
* Average Revenue Per Converted User

A visual KPI Tree was created and exported as `kpi_tree.png`.

---

## 5. Experiment Analysis Approach

The analysis was conducted in the following stages:

1. Data Quality Assessment

   * Missing values
   * Duplicate user IDs
   * Binary field validation
   * Outlier checks
   * Segment distribution checks

2. KPI Performance Comparison

   * Control vs Treatment analysis
   * Funnel performance evaluation
   * Revenue and engagement analysis

3. Segment Analysis

   * Region Analysis
   * Device Type Analysis
   * Traffic Source Analysis

4. Guardrail Analysis

   * Refund behavior
   * Support ticket impact
   * Revenue quality assessment

---

## 6. Hypothesis Test Summary

### Test Used

Two-Proportion Z-Test

### Hypotheses

**H₀ (Null Hypothesis):**
The new onboarding experience does not improve Paid Conversion Rate.

**H₁ (Alternative Hypothesis):**
The new onboarding experience improves Paid Conversion Rate.

### Results

* Z-Score: 3.41
* P-Value: 0.0003
* Significance Level (α): 0.05

### Conclusion

Since the p-value is less than 0.05, the Null Hypothesis was rejected. The improvement in Paid Conversion Rate is statistically significant and unlikely to be caused by random variation.

---

## 7. Guardrail Metrics Considered

### Refund Rate

* Control: 0.00%
* Treatment: 0.42%

### Support Ticket Rate

* Control: 14.72%
* Treatment: 24.76%

### Average Revenue Per Converted User

* Control: 1630.10
* Treatment: 770.41

Although guardrail metrics showed some deterioration, the overall business impact remained positive due to significant gains in conversion and engagement.

---

## 8. Final Recommendation

Proceed with a full rollout of the new onboarding experience.

Key reasons:

* Paid Conversion Rate more than doubled.
* User engagement improved significantly.
* Average Revenue Per User increased.
* Users converted faster.
* Statistical testing confirmed the results are significant.

Support Ticket Rate and Average Revenue Per Converted User should continue to be monitored after rollout.

---

## 9. Assumptions and Limitations

### Assumptions

* Experiment groups were randomly assigned.
* User behavior during the experiment period represents normal operating conditions.
* Revenue data accurately reflects user purchases within the 30-day observation window.

### Limitations

* Long-term customer retention was not measured.
* Customer Lifetime Value (CLV) was not available.
* Social traffic showed weaker performance and may require additional investigation.
* The analysis is limited to the metrics available in the dataset.

---

## 10. Screenshots Included

The submission includes screenshots and outputs from:

1. summary_metrics.png 
2. hypothesis_test_output.png 
3. kpi_tree_preview.png

These screenshots support the findings and recommendations presented in the project deliverables.
