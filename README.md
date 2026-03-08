#  Telecom Customer Churn Analysis & Dashboard (2024)

An Excel-based **Customer Churn Intelligence Dashboard** analyzing **4,250 telecom customers** to identify churn drivers, behavioral segments, plan impacts, and risk tiers. Built as a structured assessment project demonstrating data analysis, segmentation, and business insight communication in Microsoft Excel.

---

##  Dashboard at a Glance

| Metric | Value |
|---|---|
| Total Customers | 4,250 |
| Churned Customers | 598 |
| Overall Churn Rate | **14.07%** |
| Retention Rate | **85.93%** |

---

##  Workbook Structure

The file is organized into **4 focused sheets**:

```
Telecom_Customer_Churn_Analysis___Dashboard_Data__2024_.xlsx
│
├── Overview         → KPI summary; churned vs retained avg metrics;
│                      customer service calls vs churn rate analysis
│
├── Clusters         → K-Means behavioral cluster analysis (4 segments)
│                      by day/evening/night/international usage
│
├── Plans & Usage    → Churn by international plan, voicemail plan,
│                      day minutes usage tier, and area code
│
└── Risk Segments    → 3-tier risk scoring (Low / Medium / High)
                       with estimated churn counts per tier
```

---

##  Key Findings

### Churned vs Non-Churned — Avg Metric Comparison

| Metric | Non-Churned | Churned | Difference |
|---|---|---|---|
| Account Length (days) | 99.92 | 102.14 | +2.2 |
| Avg CS Calls | 1.44 | **2.28** | +0.84 |
| Day Minutes | 175.56 | **208.99** | +33.4 |
| Day Charge ($) | $29.84 | **$35.53** | +$5.69 |
| Evening Charge ($) | $16.88 | $17.85 | +$0.97 |

Churned customers consistently use more daytime minutes, pay higher charges, and contact customer service significantly more often.

### Customer Service Calls — The Biggest Red Flag

| CS Calls | Churn Rate |
|---|---|
| 0 | 10.9% |
| 1 | 10.9% |
| 2 | 10.8% |
| 3 | 11.3% |
| **4+** | **50.75%** |

Customers who called customer service **4 or more times** churn at **50.75%** — a **4.6× increase** over baseline. This is the single strongest churn predictor in the dataset.

### International Plan — High Risk

| Plan | Customers | Churn Rate |
|---|---|---|
| No International Plan | 3,854 | 11.2% |
| **Has International Plan** | 396 | **42.2%** |

Customers with an international plan churn at nearly **4× the rate** of those without one — strongly suggesting the plan is not meeting their needs or expectations.

### Voicemail Plan

| Plan | Customers | Churn Rate |
|---|---|---|
| No Voicemail | 1,112 | 7.4% |
| **Has Voicemail** | 3,138 | **16.4%** |

Counterintuitively, voicemail plan holders churn more. This may reflect that higher-engagement customers have more interactions — and more opportunities to become dissatisfied.

### Day Minutes Usage Tiers

| Usage Tier | Churn Rate | Risk |
|---|---|---|
| Low (<143 min) | 12.1% | Low |
| Mid-Low (143–180 min) | 9.1% | Low |
| Mid-High (180–216 min) | 6.2% | Low |
| **High (>216 min)** | **28.7%** | **High** |

Heavy daytime users churn at nearly **3× the rate** of moderate users — likely hitting plan caps or incurring overage charges.

### Behavioral Clusters (K-Means, 4 Segments)

| Cluster | Day Mins | Eve Mins | Night Mins | Intl Mins | Churn Rate | Status |
|---|---|---|---|---|---|---|
| **0** | **228** | 222 | 175 | 11.1 | **22.2%** | Priority |
| 1 | 181 | 165 | **241** | 11.9 | 11.9% | Stable |
| 2 | 126 | 222 | 180 | 10.9 | 10.9% |  Stable |
| 3 | 187 | 190 | 210 | 6.9 | 10.8% |  Stable |

**Cluster 0** (heavy daytime callers) is the only high-risk segment at **22.2% churn** — more than double the other clusters.

### Risk Tier Segmentation

| Risk Tier | Score Range | Customers | Churn Rate | Est. Churned |
|---|---|---|---|---|
| Low Risk | 0–2 | 2,689 | 2.4% | ~65 |
| Medium Risk | 3–6 | 1,338 | 32.2% | ~431 |
| **High Risk** | **7+** | **223** | **45.7%** | **~102** |

223 high-risk customers have a near coin-flip chance of churning. Medium-risk customers (1,338) represent the largest churn volume by absolute numbers.

---

##  Recommendations

1. **Trigger immediate intervention at the 3rd CS call** — With churn jumping to 50.75% at 4+ calls, a proactive outreach protocol (callback, account review, discount offer) should activate automatically when a customer logs their 3rd support call.

2. **Overhaul the international plan or create a better alternative** — A 42.2% churn rate means customers on this plan are deeply dissatisfied. Conduct exit surveys, review pricing vs. competitors, and consider introducing flexible or tiered international options.

3. **Create a high-usage day minutes plan tier** — Customers using >216 minutes/day churn at 28.7%. Offering an uncapped or higher-limit daytime plan would directly address the likely cause: bill shock or throttling.

4. **Launch a retention campaign targeting Cluster 0** — These 22.2%-churn heavy daytime callers should receive proactive plan upgrade offers and personalized outreach before they decide to leave.

5. **Focus medium-risk customers (score 3–6) for proactive retention** — They represent the highest absolute churn volume (~431 estimated). Loyalty incentives, plan reviews, or check-in calls for this group would have the greatest overall impact on reducing churn numbers.

6. **Investigate the voicemail plan paradox** — The 16.4% churn among voicemail holders vs 7.4% without warrants deeper investigation. Segmenting by usage frequency within this group could reveal whether it's the plan itself or the customer profile driving the gap.

7. **Use the risk score model for monthly at-risk reporting** — The 3-tier risk framework (Low / Medium / High) should be run monthly so account managers can prioritize outreach on customers who have recently moved into Medium or High tiers.

---

##  Tools & Methods

- **Microsoft Excel** — Data structuring, pivot analysis, charting, and dashboard design
- **K-Means Clustering** — 4-segment behavioral profiling by usage pattern (day/evening/night/international minutes)
- **Risk Scoring Model** — Composite 3-tier scoring (0–2 Low, 3–6 Medium, 7+ High) based on churn signal factors
- **Comparative Metric Analysis** — Churned vs retained cohort comparison across 7 variables
- **Churn Rate Segmentation** — Breakdown by plan type, usage tier, CS call frequency, and area code

---

## Author

**Mohd Faiz**
- **Role:** Business and Data Analyst
- **GitHub:** [https://github.com/faizikbal01-lab](https://github.com/your-username)



#
