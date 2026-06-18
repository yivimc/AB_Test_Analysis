# A/B Test Analysis Report
**E-Commerce Landing Page Experiment**

---

## 1. Background & Hypothesis

An e-commerce platform tested a new landing page design to evaluate whether 
it could improve user conversion rate.

- **Null Hypothesis (H₀):** The new page has no effect on conversion rate
- **Alternative Hypothesis (H₁):** The new page changes conversion rate
- **Significance Level:** α = 0.05
- **Statistical Power:** 80%

---

## 2. Data Overview

| Item | Value |
|------|-------|
| Raw records | 294,478 |
| Records removed (mismatch + duplicates) | 3,894 |
| Final records | 290,584 |
| Control group size | 145,274 |
| Treatment group size | 145,310 |
| Experiment duration | 22 days |

---

## 3. Validity Checks

Before running the hypothesis test, three validity checks were performed 
to ensure experimental integrity.

### 3.1 Sample Ratio Mismatch (SRM)
A chi-square test confirmed that the 50/50 split was maintained correctly.

- Chi² = 0.0045, p = 0.9468
- **Result: No SRM detected ✅**

### 3.2 Power Analysis
Based on the baseline conversion rate (12.04%) and a minimum detectable 
effect (MDE) of 1%, the required sample size per group was 17,208.  
With 145,274 users per group, the experiment was **sufficiently powered ✅**

### 3.3 Time Distribution
Both groups showed consistent daily user counts throughout the experiment 
period, confirming no time-based sampling bias **✅**

---

## 4. Hypothesis Testing Results

### 4.1 Conversion Rates

| Group | Conversion Rate | 95% Confidence Interval |
|-------|----------------|------------------------|
| Control | 12.04% | (11.87%, 12.21%) |
| Treatment | 11.88% | (11.71%, 12.05%) |
| Difference | -0.16pp | — |
| Relative Change | -1.31% | — |

### 4.2 Statistical Test

- **Test:** Two-proportion Z-test (two-tailed)
- **Z-statistic:** -1.3109
- **P-value:** 0.1899
- **Result:** Fail to reject H₀ (p > 0.05)

### 4.3 Effect Size

- **Cohen's h:** -0.0049
- **Magnitude:** Negligible
- The difference is not only statistically insignificant but also 
  practically meaningless from a business perspective.

---

## 5. Segmentation Analysis

### 5.1 Novelty Effect Check
Cumulative conversion rates for both groups converged quickly and remained 
stable throughout the experiment, indicating **no novelty effect**.

### 5.2 Weekday Analysis
No consistent pattern of treatment outperforming control was observed 
across any day of the week.

### 5.3 Hourly Analysis
Conversion rate trends by hour of day were largely parallel between groups, 
with no time window showing a meaningful treatment advantage.

---

## 6. Conclusion & Recommendation

| Question | Answer |
|----------|--------|
| Is the difference statistically significant? | No (p = 0.19) |
| Is the effect size meaningful? | No (Cohen's h ≈ 0) |
| Did the experiment run long enough? |  Yes (converged, no novelty effect) |
| Was the experiment set up correctly? |  Yes (no SRM, balanced groups) |

**Recommendation: Do not launch the new landing page.**

The new page shows a -1.31% relative decrease in conversion rate. 
While this did not reach statistical significance, there is no evidence 
of any positive effect. Given the experimental validity was confirmed 
at every check, the result is reliable. The team should consider 
redesigning the page with clearer hypotheses about which elements 
drive conversion.