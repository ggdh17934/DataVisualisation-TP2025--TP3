# TP3 — Required EDA answers

Data: 48,204 UCI hourly records, kept in their original form for the requested EDA.
The literal holiday value 'None' is preserved as a category. No optional interactive bonus is included.

## Descriptive statistics

Mean: **3259.82**; median: **3380.00**; mode(s): **[353, 356]** cars/hour.
Standard deviation: **1986.86**; range: **7280** cars/hour.
The median exceeds the mean, suggesting negative (left) skew.
The measured skewness is **-0.0894** (negative, modest in magnitude),
which is consistent with that direction; the histogram also reveals a mixture
of low/high traffic periods, so a single skewness value does not describe all its structure.
Excess kurtosis is **-1.3091**: platykurtic (lower excess kurtosis than normal).
Pandas reports excess kurtosis, whose normal reference value is 0, not 3.

Highest weather mean: **Clouds**, 3618.45.
Highest weather standard deviation: **Fog**, 2125.53.
Group counts are included because small groups can have unstable summaries.

## Distribution, spread, and holidays

Q1 = **1193.00**, Q3 = **4933.00**, IQR = Q3 − Q1 = **3740.00** cars/hour.
This large central spread agrees with substantial hourly variability.
All named holiday categories are shown beside ordinary ('None') observations,
with the same neutral color: their medians and spreads can be compared by
position without relying on hue. The grouped table gives actual values/counts.
Ordinary records have standard deviation 1986.26,
whereas the named-holiday groups range from
31.55 to 277.11:
their observed spread is much smaller, and their medians are also lower.
Named holiday samples are sparse and often identify a particular holiday hour,
so apparent differences are descriptive, not proof of a statistically significant
whole-day holiday effect. No unrequested significance test is added.

## Correlation and the causation question

The strongest absolute environmental correlation with traffic is **temp**,
with Pearson r = **0.1303** (positive).
It is still weak, despite being the strongest of the four measured relationships.
Correlation does not establish causation: time of day, commuting schedules,
weekday/weekend differences and season can affect both weather readings and traffic.
For example, daytime can be warmer and busier because people commute, rather
than warmth itself causing traffic. Aggregating these different groups can
mask or alter within-group relationships (the concern behind Simpson's paradox);
this dataset summary alone does not prove an actual reversal.

Assignment: https://github.com/ahmed3991/DataVisualisation-TP2025/blob/main/TP3/TP3.md
Data: https://archive.ics.uci.edu/dataset/492/metro+interstate+traffic+volume
