# Healthcare-associated-infections
Hospitals Healthcare-associated infections in the united states for the periode between Jan-2018 and Dec-2019

original Dataset downloaded from https://data.medicare.gov which is a national health insurance program in the United States,
 begun in 1966 under the Social Security Administration (SSA) and now administered by the Centers for Medicare and Medicaid Services (CMS).
 
In our explanatory analysis, I tried to put only the plots that can answer our questions (in the introduction section), for further explorations please have a look at the exploratory_analysis notebook or html file.

our slides were created with nbconvert using the following code:
jupyter nbconvert explanatory_analysis.ipynb --to slides --post serve --template output_toggle

if you try this please don't forget to put the plotly.js in the same directory, otherwise the plotly geo heatmap willnot be rendered in the slides.

to sumup our findings:

HAI_6 is the most common infection, and the HAI_3, HAI_4 are the least common.

Hospitals are benchmarked according to their ability to predict and manage the observed infection cases, Opposed to the worse benchmarked, The best benchmarked facilities have a lower ratio interval and mean, high patient days or operations, a low confidence levels with a highly predicted cases but a lower observed cases mean.

Compared to the normal hospitals, the lower confidence level of the best benchmarked ones have less median and interquartile values, their maximum values are less than the normal max which is around 1. Contrarily the minimum of the Worst benchmarked hospitals is 1, their medians and IQR are higher and a much higher outliers. For the upper confidence level, The max of the best hospitals around the min of the normal ones and have a much smaller IQR, the min of the worst hospitals is around the median of the normal ones and have a higher IQR.

The Medians and interquartiles of the best benchmarked hospitals for the Number of patient days or operations and predicted cases are higher than the normal and the worst hospitals, however the observed cases are less than the predicted ones,therefore a lower ratio with a lower IQR values and a maximum not exceeding the normal median opposed to the worst hospitals who have a minimum ratio bigger than the normal Q3 upper quartile.
