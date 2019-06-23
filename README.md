# hospital-readmit
Springboard project for EDA and hypothesis testing in Python.

**Background:**

In October 2012, the US government's Center for Medicare and Medicaid Services (CMS) began reducing Medicare payments for Inpatient Prospective Payment System hospitals with excess readmissions. Excess readmissions are measured by a ratio, by dividing a hospital’s number of “predicted” 30-day readmissions for heart attack, heart failure, and pneumonia by the number that would be “expected,” based on an average hospital with similar patients. A ratio greater than 1 indicates excess readmissions.

Code: EDA_hospital_readmit/iderule_dsi_inferential_statistics_exercise_3.ipynb

Data: EDA_hospital_readmit/data

**Results:**

The hypothesis test for the slop rejected the null hypothesis at 𝛼 = .01. The results were:

  * slope: -2.9010517330570697e-05
  * intercept: 1.018106147373357
  * r-value: -0.09739794351079352
  * p-value: 1.2225473776734486e-25
  * standard error: 2.7649127349110587e-06
  
The p-value was incredibly small and arbitrarily close to zero. The slope was also effectively zero. This along with the r-value points to no correlation between the number of discharges and the excess readmissions ratio. Furthermore:

  * Confidence Interval of the slope: -2.9139931220248926e-05 to -2.888110344089247e-05
  * Margin of Error of the slope is: 1.2941388967822846e-05 %
  
This is more support for the null hypothesis since the margin of error is small, but the confidence interval does not include zero. This is negligigle since the slope is so small, that for this case it is effectively zero. The low r-value also point to this being a poor correlation.

This is statistically significant and practically significant. The first analysis reported that there is a significant correlation between the two variables and made recommendations based on that conclusion. Since the methods they used for that conclusion were wrong, and there is not a correlation, the recommendations need to be changed.

"Hospitals/facilties with small capacity (< 300) should be required to demonstrate upgraded resource allocation for quality care to continue operation." This recommendation does is not supported by any analysis now, so it can not be used.

"Directives and incentives should be provided for consolidation of hospitals and facilities to have a smaller number of them with higher capacity and number of discharges." This recommendation is also not supported anymore from the above analyses.

There is a chance that these recommendations would help, because they fix other lurking variables, but that notion is not supported or explored here.

