# Megaline Prepaid Plans: Statistical Revenue Analysis

## Objective
Acting as an analyst for the telecommunications company Megaline, the purpose of this project was to examine the consumption profiles and revenues of 500 users. The strategic business question was to determine which prepaid plan (Surf or Ultimate) generates higher total revenue, allowing the commercial department to optimize and adjust its advertising budget.

## Key Results
The analysis revealed that while the Ultimate plan has a higher flat monthly fee, the **Surf plan generates substantial additional revenue**. This occurs because Surf users frequently exceed their package limits for data and minutes, triggering expensive overage fees. Through formal hypothesis testing, it was statistically proven that the average revenues of the two plans differ significantly, confirming Surf as a highly dynamic revenue generator.

## Tools & Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **SciPy** (Statistical Module for Hypothesis Testing)
- **Data Wrangling** (Aggregating multiple logs of calls, internet data, and messaging)

## What I Learned
- Consolidating and engineering complex corporate data distributed across multiple independent transaction tables.
- Analytic data cleaning, such as handling zero-duration calls and commercial rounding of internet data traffic.
- Formulating null ($H_0$) and alternative ($H_1$) hypotheses, and applying the Student's t-test for independent samples with unequal variances (Welch's t-test).

## Future Improvements
- Conduct a price elasticity analysis to evaluate if adjusting Surf's overage fees would increase revenue or trigger customer churn.
- Build a temporal cohort analysis to track faturamento evolution based on user account age.

---

## Methodology
1. **Data Aggregation:** Combined monthly minutes, messages, and gigabytes consumed per unique client.
2. **Anomaly Treatment:** Handled data types, missing records, and consumption outliers.
3. **Distribution Analysis:** Plotted histograms and calculated means, variances, and standard deviations of monthly consumption per plan.
4. **Statistical Validation:** Ran t-tests to evaluate population means based on the calculated $p$-value.

## How to Run
1. Clone this repository.
2. Install the required dependencies: `pip install pandas numpy scipy matplotlib seaborn`
3. Execute the notebook to review the full financial and consumption report.
