# Project Title

## 1. Research Question

Which U.S. counties have higher quality daycare providers, and which factors seem related to daycare quality?  This matters because for working parents, childcare is essential and the cost of childcare is significant.

## 2. Hypothesis

I expect that mean_overall_stars will show a higher rating for daycare providers in Minnesota Twin Cities zip codes than other areas, such as rural Southern Nevada zip codes.

Null hypothesis: Zip code labels are unrelated to daycare quality scores (mean_overall_stars).

## 3. Data Description

Describe your data source(s):

* Where it comes from (URL, API, dataset name)
    https://childery.com/data
    I found this as one of the GitHub awesome-public-datasets
* What each observation represents (unit of analysis)
    Each row represents a "Zip Code Tabulation Area" in the U.S.  Essentially, daycare providers are being grouped by zip code and then the zip code is assessed as a whole for daycare quality and daycare features.
* Number of observations and key variables
    21k observations.  Key variables:
        **zcta**: 5-digit ZIP Code Tabulation Area
        **providers_total**: Count of active licensed daycares in the ZCTA
        **mean_overall_stars**: Mean of Childery's 1-5 Overall rating across providers with a rating
        **mean_process_stars**: Mean of Process subscore (QRIS + NAEYC + CLASS)
        **mean_structural_stars**: Mean of Structural subscore (state regulatory baseline)
        **pct_naeyc_accredited**: Share NAEYC-accredited


* Any filtering, cleaning, or transformation steps
        Some zip codes have their data suppressed if there are less than 5 providers within a zip code.

## 4. Methods

Summarize how you analyzed the data:

* The test statistic for your permutation test
* How you simulated or resampled under the null hypothesis
* The metric(s) for which you created bootstrap confidence intervals
* Why the CLT does not apply to at least one metric

## 5. Results

Present your main findings:

* Key summary statistics and visualizations
* Observed test statistic and p-value (if applicable)
* Bootstrap confidence intervals for relevant metrics

## 6. Uncertainty Estimation

Discuss your resampling results:

* How many resamples you used
* What the bootstrap or randomization distributions looked like
* How you interpret the interval estimates

## 7. Limitations

Briefly note any limitations in data, assumptions, or methods, including sources of bias or missing data.

## 8. References

List all datasets, tools, libraries, or papers you cited.

---

**Reminder:** Your README should be clear enough that someone unfamiliar with your work could understand what you studied, how you analyzed it, and what you found.
